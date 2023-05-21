<h1 align="center">Examen-JEE</h1>
<br>
<hr>
<h4 align="center">
(https://drive.google.com/file/d/1qWerutsnH4z7Qbf9Uqx_V-FS4Njq-k6w/view?usp=share_link)
</h4>
   <hr>


```markdown
# Application de Gestion de Conférences

Il s'agit d'une application web Java Enterprise Edition (JEE) pour gérer les conférences et les sessions. L'application suit des règles métier spécifiques et des exigences techniques.
```
<h1 align="center">Questions de concepts QCM</h1>

```markdown
## Questions de concepts QCM

1. Quelle est la relation qui existe entre JPA et Hibernate ?
   - A. JPA est une API et Hibernate est une implémentation de JPA
   - B. Hibernate est une API et JPA est un Framework qui implémente JPA
   - C. JPA est un Framework alors que Hibernate non
   - D. Aucune relation entre JPA et Hibernate
   - **Réponse : A. JPA est une API et Hibernate est une implémentation de JPA**

2. En conception logiciel, que signifie le couplage faible ?
   - A. Lier une classe A à une classe B
   - B. Lier une classe A à une classe IB
   - C. Implémenter deux interfaces IA et IB
   - D. Hériter d’une classe abstraite
   - **Réponse : C. Implémenter deux interfaces IA et IB**

3. Quelles sont les deux annotations JPA qui sont obligatoires pour créer une entité JPA ?
   - A. @Entity
   - B. @Id
   - C. @Data
   - D. @NoArgConstructor
   - **Réponse :**
     - @Entity
     - @Id

4. Dans Spring, quelle est la façon la plus recommandée pour faire l’injection des dépendances ?
   - A. En utilisant l’annotation @Autowired
   - B. En utilisant un constructeur
   - C. En utilisant les Setters
   - **Réponse : B. En utilisant un constructeur**

5. Dans Spring, quelle est l’annotation qui permet de faire l’injection des dépendances ?
   - A. @InjectDependency
   - B. @Autowired
   - C. @Dependency
   - **Réponse : B. @Autowired**

6. Quelle annotation à utiliser sur une méthode d’un contrôleur Spring MVC pour qu'elle soit exécutée quand une requête HTTP est envoyée par la méthode GET avec le path "/index" ?
   - A. @GetMapping(path="/index")
   - B. @GetHttpMapping(path="/index")
   - C. @HttpGet(path="/index")
   - D. @RequestMapping(value="/index", method=HttpMethod.GET)
   - **Réponse : A. @GetMapping(path="/index")**

7. Quelle annotation permet de marquer une classe comme étant un contrôleur Spring MVC ?
   - A. @Dispatche
   - B. @Controller
   - C. @MvcController
   - D. @DispatcherController
   - **Réponse : B. @Controller**

8. Dans une application Spring Boot utilisant Spring Data JPA, quelle est l’annotation qui permet de déléguer à Spring la gestion des transactions ?
   - A. @Transactional
   - B. @UseTrandaction
   - C. @SpringTransaction
   - D. @DataTransactional
   - **Réponse : A. @Transactional**

9. Dans une vue basée sur Thymeleaf, comment créer un lien hypertexte vers l'action "/detail" en envoyant avec le lien deux paramètres x et y dont les valeurs se trouvent dans les variables x et y d'un objet p du contexte ?
   - A. <a th:href="/detail?x=${p.x}&y=${p.y}">Details</a>
   - B. <a th:href="@{/detail(x=${p.x} & y=${p.y})}">Details</a>
   - C. <a th:href="@{/detail(x=${p.x},y=${p.y})}">Details</a>
   - D. <a th:href="@{/detail(x,y=${p.x, p.y})}">Details</a>
   - **Réponse : C. <a th:href="@{/detail(x=${p.x},y=${p.y})}">Details</a>**

10. Dans le rôle des DTO dans une application web ?
    - A. Transférer les données vers la base de données
    - B. Transférer les données entre la couche UI web et les entités JPA
    - C. Sécuriser les données
    - D. Rendre les données persistantes
    - **Réponse : B. Transférer les données entre la couche UI web et les entités JPA**

11. On suppose qu’une classe A est liée à une classe B par une association de type OneToMany avec le mode fetch = EAGER. Qu'est-ce qui se passera si on demande à Hibernate de charger un objet de type A ?
    - A. Hibernate va charger en mémoire uniquement un objet de la classe A
    - B. Hibernate va charger en mémoire un objet de la classe A et tous les objets B qui sont liés à A
    - C. Hibernate va charger en mémoire un objet de la classe B et tous les objets A qui sont liés à B
    - D. Hibernate va charger en mémoire uniquement un objet de la classe B qui est lié à A
    - **Réponse : B. Hibernate va charger en mémoire un objet de la classe A et tous les objets B qui sont liés à A**

12. On suppose que les classes A, B et C héritent de la classe abstraite D. Dans JPA, en utilisant la stratégie SINGLE_TABLE pour mapper l'héritage, Hibernate va générer les tables suivantes dans la base de données :
    - A. Trois tables représentant les classes A, B et C
    - B. Quatre tables représentant les classes A, B, C et D
    - C. Une seule table qui contient tous les attributs des 4 classes A, B, C et D
    - D. Une seule table qui contient tous les attributs des 3 classes A, B, C
    - **Réponse : C. Une seule table qui contient tous les attributs des 4 classes A, B, C et D**

13. On suppose que les classes A, B et C héritent de la classe abstraite D. Dans JPA, quelle est la stratégie de mapping de l'héritage qui va entraîner la génération de 4 tables dans la base de données :
    - A. La stratégie SINGLE_TABLE
    - B. La stratégie TABLE_PER_CLASS
    - C. La stratégie JOINED_TABLE
    - D. Aucune de ces trois
    - **Réponse : B. La stratégie JOINED_TABLE**

```

## Règles Métier

- Une session est composée de plusieurs conférences et est animée par un modérateur dans une salle spécifique.
- Chaque conférence est animée par un intervenant (speaker).
- Les participants peuvent s'inscrire à plusieurs sessions.
- Les participants peuvent poster des commentaires pour chaque conférence (invités, intervenants ou modérateurs).

## Exigences Techniques

- Les données sont stockées dans une base de données MySQL ou H2.
- L'application est composée de trois couches :
  - La couche DAO basée sur Spring Data, JPA, Hibernate et JDBC.
  - La couche métier (interfaces et implémentations).
  - La couche DTO avec des mappeurs DTO/Entités.
  - La couche web basée sur Spring MVC avec une interface utilisateur utilisant Angular ou Thymeleaf.
- L'inversion de contrôle (IoC) est mise en œuvre avec Spring IOC.
- La sécurité est mise en œuvre avec Spring Security.

## Implémentation

### Couche DAO

- Écrire le code des entités JPA de l'application en utilisant les annotations Lombok.
- Écrire le code des interfaces JPA Repository basées sur Spring Data pour chaque entité.



# a) Code des entités JPA de l'application:

```markdown

```java
import javax.persistence.*;

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Session {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private String name;
    
}

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Conference {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private String title;
    private LocalDate date;
    private LocalTime startTime;
    private LocalTime endTime;
    private String description;
    
    // Relationship mappings
    
    @ManyToOne
    private Session session;
    
    @ManyToOne
    private Speaker speaker;
    
}

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Room {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private String name;
    
}

@Entity
@Inheritance(strategy = InheritanceType.SINGLE_TABLE)
@DiscriminatorColumn(name = "TYPE",length = 1)
@Data @NoArgsConstructor @AllArgsConstructor
public class Participant {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private String name;
    private String email;
    private String photo;
    private String gender;
    
}

@Entity
@DiscriminatorValue("M")
@Data @NoArgsConstructor @AllArgsConstructor
public class Moderator extends Participant {
    private String specialty;
    
}

@Entity
@DiscriminatorValue("S")
@Data @NoArgsConstructor @AllArgsConstructor
public class Speaker extends Participant {
    private String profileLink;
    
}

@Entity
@DiscriminatorValue("G")
@Data @NoArgsConstructor @AllArgsConstructor
public class Guest extends Participant {
    private String affiliation;
    
}

@Entity
@Data @NoArgsConstructor @AllArgsConstructor
public class Registration {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private LocalDate date;
    private String status;
    private double price;
    
    // Relationship mappings
    
    @ManyToOne
    private Participant participant;
    
    @ManyToOne
    private Session session;
    
}

@Entity
@Data @NoArgsConstructor @AllArgsConstructor
public class Comment {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private LocalDate date;
    private String content;
    private int likes;
    
    // Relationship mappings
    
    @ManyToOne
    private Conference conference;
    
    @ManyToOne
    private Participant participant;
    
}

```



# b) Code des interfaces JPA Repository basées sur Spring Data:

```markdown


```java
import org.springframework.data.jpa.repository.JpaRepository;

public interface SessionRepository extends JpaRepository<Session, Long> {
}

public interface ConferenceRepository extends JpaRepository<Conference, Long> {
    List<Conference> findBySpeaker(Speaker speaker);
}

public interface RoomRepository extends JpaRepository<Room, Long> {
}

public interface ParticipantRepository extends JpaRepository<Participant, Long> {
}

public interface RegistrationRepository extends JpaRepository<Registration, Long> {
}

public interface CommentRepository extends JpaRepository<Comment, Long> {
}
```



### Couche Métier

- Écrire le code de l'interface `IConferenceService` pour gérer l'ajout de conférences et la consultation des conférences animées par un intervenant donné.
- Écrire le code d'une implémentation de cette interface.

# a) Code de l'interface IConferenceService:

```java
import java.util.List;

public interface IConferenceService {
    Conference addConference(Conference conference);
    List<Conference> getConferencesBySpeaker(Speaker speaker);
}
```

# b) Code d'une implémentation de l'interface IConferenceService:

```java
import org.springframework.stereotype.Service;
import java.util.List;

@Service
@AllArgsConstructor
public class ConferenceServiceImpl implements IConferenceService {
    
    private ConferenceRepository conferenceRepository;

    @Override
    public Conference addConference(Conference conference) {
        return conferenceRepository.save(conference);
    }

    @Override
    public List<Conference> getConferencesBySpeaker(Speaker speaker) {
        return conferenceRepository.findBySpeaker(speaker);
    }
}

```



### Couche Web

- Créer le service web RESTful pour gérer les sessions et les conférences.
- Implémenter les points de terminaison (endpoints) nécessaires pour effectuer les opérations CRUD.

# a) Web service RESTful pour gérer les sessions et les conférences. Voici un exemple de code pour une API REST utilisant Spring MVC:

```java
@RestController
@AllArgsConstructor
public class SessionController {

    private SessionRepository sessionRepository;

    @GetMapping("/sessions")
    public List<Session> getAllSessions() {
        return sessionRepository.findAll();
    }

    @PostMapping("/sessions")
    public Session createSession(@RequestBody Session session) {
        return sessionRepository.save(session);
    }

}

@RestController
@AllArgsConstructor
public class ConferenceController {

    private ConferenceRepository conferenceRepository;

    @GetMapping("/conferences")
    public List<Conference> getAllConferences() {
        return conferenceRepository.findAll();
    }

    @PostMapping("/conferences")
    public Conference createConference(@RequestBody Conference conference) {
        return conferenceRepository.save(conference);
    }

}

```



### Sécurité

Pour sécuriser l'accès à l'application en utilisant Spring Security avec un système d'authentification des utilisateurs et trois types de rôles (ROLE_CLIENT, ROLE_EMPLOYE, ROLE_ADMIN), voici les étapes à suivre :

# 1- Ajouter les dépendances Spring Security dans le fichier de configuration Maven "pom.xml".

# 2- Créer une classe de configuration pour Spring Security.


```java
@Configuration
@EnableWebSecurity
public class SecurityConfig extends WebSecurityConfigurerAdapter {

     @Autowired
     private PasswordEncoder passwordEncoder;
    
    
    @Bean
    public InMemoryUserDetailsManager inMemoryUserDetailsManager(){
        return new InMemoryUserDetailsManager(
                User.withUsername("employe").password(passwordEncoder.encode("1234")).roles("EMPLOYE").build(),
                User.withUsername("client").password(passwordEncoder.encode("1234")).roles("CLIENT").build(),
                User.withUsername("admin").password(passwordEncoder.encode("1234")).roles("CLIENT","EMPLOYE","ADMIN").build()


        );
    }
  
  // Injecter le service de détails utilisateur personnalisé
  
  @Bean
  protected void configure(HttpSecurity httpSecurity) throws Exception {
    httpSecurity.authorizeHttpRequests().requestMatchers("/admin/**").hasRole("ROLE_ADMIN")
    httpSecurity.authorizeHttpRequests().requestMatchers("/employe/**").hasAnyRole("ROLE_EMPLOYE", "ROLE_ADMIN")
    httpSecurity.authorizeHttpRequests().requestMatchers("/client/**").hasAnyRole("ROLE_CLIENT", "ROLE_EMPLOYE", "ROLE_ADMIN")
        return httpSecurity.build();
  }
  
}

```
