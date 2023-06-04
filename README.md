<h1 align="center">Examen-JEE</h1>
<br>
<hr>
<h4 align="center">
   Exemple 1 : <br>
(https://drive.google.com/file/d/1qWerutsnH4z7Qbf9Uqx_V-FS4Njq-k6w/view?usp=share_link)
 <br><br><br><br> Exemple 2 : <br>
(https://drive.google.com/file/d/1aro8w_w1Vy4eybLrP7ad1iShXJgJH9sB/view?usp=drive_link)
</h4>
   <hr>

# Exemple 1 : (Solution)

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

```markdown
# Conception :

`Session`
- id
- nom
- modérateur: Modérateur (1 session est animée par 1 modérateur)
- salle: Salle (1 session se déroule dans 1 salle)
- conférences: List<Conférence> (1 session se compose de plusieurs conférences)

`Conférence`
- id
- titre
- date
- heureDébut
- heureFin
- description
- speaker: Speaker (1 conférence est animée par 1 speaker)
- commentaires: List<Commentaire> (1 conférence peut avoir plusieurs commentaires)

`Salle`
- id
- nom

`Participant`
- id
- nom
- email
- photo
- genre

`Modérateur`
- spécialité
- session: Session (1 modérateur anime 1 session)

`Invité`
- affiliation
- inscriptions: List<Inscription> (1 invité peut effectuer plusieurs inscriptions)

`Speaker`
- profilPro
- conférences: List<Conférence> (1 speaker peut animer plusieurs conférences)

`Inscription`
- id
- date
- statut
- prix
- session: Session (1 inscription concerne 1 session)
- invité: Invité (1 inscription est effectuée par 1 invité)

`Commentaire`
- id
- date
- contenu
- likes
- conférence: Conférence (1 commentaire concerne 1 conférence)
- participant: Participant (1 commentaire est posté par 1 participant)
```
``` markdown
# Architecture Technique :

+---------------------+
|                     |
|    Base de données  |
|    (SGBD)           |
|                     |
+---------------------+
          |
          |
+------------------------+
|                        |
|    Couche Backend      |
|    (Spring Boot,       |
|     Hibernate)         |
|                        |
+------------------------+
          |
          |
+------------------------+
|                        |
|   API REST             |
|    (Communication avec |
|     le Front)          |
|   (Restful API)        |
|                        |
+------------------------+
          |
          |
+------------------------+
|                        |
|   Couche Frontend      |
| (Thymeleaf ou Angular) |
|                        |
+------------------------+


```

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

<hr>

# Exemple 2 : (Solution)

```markdown
# Application de gestion de consultations médicales

L'objectif de cette application est de développer un système basé sur le Spring Framework permettant de gérer les consultations relatives aux rendez-vous des patients chez les médecins. Chaque patient peut effectuer plusieurs rendez-vous, chaque rendez-vous étant associé à un médecin spécifique. Chaque rendez-vous est lié à une seule consultation, et chaque consultation est liée à un seul rendez-vous.
```

```markdown

## Questions de concepts QCM

1. Si la couche métier d’une application est orientée objet et les données de l’application sont stockées dans des Système de Gestion de Base de Données Relationnelles comme MySQL, l’opération suivante s’impose :
   A. Le Mapping Objet Document
   B. Le Mapping Objet Relationnel
   C. Le Mapping Objet XML
   D. Le Mapping Objet JSON

   **Réponse : B. Le Mapping Objet Relationnel**

2. Quelles définitions qui sont correctes qui vous semble plus appropriée à JPA ?
   A. JPA est une API de persistances des objets JAVA dans des SGBD relationnelles
   B. JPA est une spécification Java/JEE qui définit un ensemble d’interfaces, d’annotations et de classes qui permet de standardiser le mapping objet relationnelle pour les applications Java/JEE
   C. JPA est une API de gestion de la sécurité
   D. JPA est un standard pour les systèmes distribués Java

   **Réponse :  A. JPA est une API de persistances des objets JAVA dans des SGBD relationnelles et B. JPA est une spécification Java/JEE qui définit un ensemble d’interfaces, d’annotations et de classes qui permet de standardiser le mapping objet relationnelle pour les applications Java/JEE**

3. Dans Spring, quelle est l’annotation qui permet de faire l’injection des dépendances ?
   A. @Inject
   B. @DependencyInject
   C. @Autowired
   D. @AutoInject

   **Réponse : C. @Autowired**

4. Quelle est l’implémentation de référence de JPA ?
   A. Hibernate
   B. Toplink
   C. EclipseLink
   D. IBatis

   **Réponse : A. Hibernate**

5. Quelle est la relation qui existe entre JPA et Hibernate ?
   A. JPA est une API et Hibernate et une implémentation de JPA
   B. Hibernate est une API et JPA est un Framework qui implémente JPA
   C. Aucune relation entre JPA et Hibernate

   **Réponse : A. JPA est une API et Hibernate et une implémentation de JPA**

6. Quelles sont les deux annotations JPA qui sont obligatoires pour créer une entité JPA ?
   A. @JPAEntity
   B. @Entity
   C. @Id
   D. @Table

   **Réponse : B. @Entity, C. @Id**

7. Dans JPA, quelle est l’annotation qui permet de désigner un attribut d’une entité JPA comme clé primaire de la table correspondante ?
   A. @PrimaryKey
   B. @KeyIdentifier
   C. @Identifier
   D. Id

   **Réponse : D. @Id**

8. Dans JPA, quelle est l’annotation qui permet de spécifier que la valeur de l’identifiant d’une entité JPA est générée automatiquement par le SGBD pour chaque nouvel enregistrement de la table correspondant à cette entité JPA?
   A. @AutoIncrement
   B. @GenerateValue
   C. @GeneratedValue
   D. @Identity

   **Réponse : C. @GeneratedValue**

9. Dans une application Spring Boot utilisant Spring Data JPA, quelle est l’annotation qui permet de délégu

er à Spring la gestion des transactions ?
   A. @UseTransactions
   B. @Transactional
   C. @Transact

   **Réponse : B. @Transactional**

10. Comment déployer une servlet ?
    A. En la déclarant dans le fichier web.xml
    B. En la déclarant dans le fichier web-deploy.xml
    C. En la déclarant dans le fichier web-deployment.xml
    D. En utilisant l’annotation @WebServlet

    **Réponse : D. En utilisant l’annotation @WebServlet**

11. Quelle annotation permet de marquer une classe comme étant un contrôleur Spring MVC ?
    A. @Controller
    B. @WebController
    C. @RequestController
    D. @DispatcherController

    **Réponse : A. @Controller**

12. Quelle annotation à utiliser sur une méthode pour que celle-ci soit exécutée quand une requête http est envoyée par la méthode GET avec le path « /index » ?
    A. @GetMapping(path="/index")
    B. @Get(path="/index")
    C. @GetHttpMapping(path="/index")
    D. @RequestMapping(value="/index", method=HttpMethod.GET)

    **Réponse : A. @GetMapping(path="/index")**

13. Quelle est l’annotation à utiliser sur un paramètre p de la méthode d’un contrôleur pour associer à un paramètre p la valeur transmise comme paramètre URL. La méthode est précédée par l’annotation @GetMapping(path="/search") et l’url est sous la forme http://localhost:8080/search?keyword=az
    A. @PathParameter(name="keyword") String p
    B. @PathVariable(name="keyword") String p
    C. @RequestParam (name="keyword") String p
    D. @PathParameter(name="keyword") String p

    **Réponse : A. @RequestParam (name="keyword") String p**

14. Dans une vue basée sur thymeleaf, comment créer un lien hypertexte vers l’action /detail en envoyant avec le line deux paramètres x et y dont les valeurs se trouvent dans les variables x et y d’un objet p du contexte ?
    A. <a th:href="@{/detail(x=${p.x},y=${p.y})}"> Details</a>
    B. <a th:href="/detail?x=${p.x}&y=${p.y}"> Details</a>
    C. <a th:href="@{/detail(x=${p.x} & y=${p.y})}"> Details</a>
    D. <a th:href="@{/detail(x,y=${p.x, p.y})}"> Details</a>

    **Réponse : A. <a th:href="@{/detail(x=${p.x},y=${p.y})}"> Details</a>**

15. Dans la sécurité Web, Que signifie le type d’attaque CSRF ?
    A. Cross Sheet Request Foreign
    B. Cross Site Request Forgery
    C. Cross Security Request Forgery

    **Réponse : B. Cross Site Request Forgery**


```

## Règles Métier

- Un patient peut effectuer plusieurs rendez-vous chez des médecins.
- Chaque rendez-vous est associé à une seule consultation.
- Chaque consultation concerne un seul rendez-vous.
- Chaque patient est défini par son identifiant, son nom, son email et sa date de naissance.
- Chaque médecin est défini par son identifiant, son nom et sa spécialité.
- Chaque rendez-vous est défini par son identifiant, sa date et un attribut indiquant s'il est annulé ou non.
- Chaque consultation est définie par son identifiant, sa description, le traitement prescrit et le type de consultation (présentielle ou distantielle).

```markdown
# 1. Diagramme de classes des entités avec les attributs :

`Patient`
- id : int
- nom : string
- email : string
- dateNaissance : date

`Medecin`
- id : int
- nom : string
- specialite : string

`RendezVous`
- id : int
- date : date
- annule : bool

`Consultation`
- id : int
- description : string
- traitementPrescrit : string
- typeConsultation : string
```
```markdown
# 2. Modèle logique de données relationnel avec les tables et les relations :


Table: `Patient`
- id (PK, int)
- nom (string)
- email (string)
- dateNaissance (date)

Table: `Medecin`
- id (PK, int)
- nom (string)
- specialite (string)

Table: `RendezVous`
- id (PK, int)
- date (date)
- annule (bool)
- patientId (FK, int)
- medecinId (FK, int)

Table: `Consultation`
- id (PK, int)
- description (string)
- traitementPrescrit (string)
- typeConsultation (string)
- rendezVousId (FK, int)
- 

### Relations :
- Patient (1) ---- (*) RendezVous
- Medecin (1) ---- (*) RendezVous
- RendezVous (1) ---- (1) Consultation

```

## Exigences Techniques

- Les données sont stockées dans une base de données MySQL ou H2
- L’application se compose de trois couches :
- La couche DAO qui est basée sur Spring Data, JPA, Hibernate et JDBC.
- La couche métier (Interfaces et implémentations)
- La couche Web basée sur Spring MVC Coté Serveur avec thymeleaf comme moteur de templates.
- L’inversion de contrôle est basée sur Spring IOC.
- La sécurité est basée sur Spring Security

## Implémentation

### Couche DAO

- Écrire le code des entités JPA de l'application en utilisant les annotations Lombok.
- Écrire le code des interfaces JPA Repository basées sur Spring Data pour chaque entité.



# a) Code des entités JPA de l'application: (Patient, Medecin, Rendez-vous et Consultation) :

```java
import lombok.*;

import javax.persistence.*;

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Patient {
    @Id
    private int id;
    private String nom;
    private String email;
    private LocalDate dateNaissance;
    @OneToMany
    private List<Patient> patient;
}

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Medecin {
    @Id
    private int id;
    private String nom;
    private String specialite;
    @OneToMany
    private List<RendezVous> rendezVous;
}

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class RendezVous {
    @Id
    private int id;
    private LocalDate date;
    private boolean annule;
    @ManyToOne
    private Patient patient;
    @ManyToOne
    private Medecin medecin;
    @OneToOne
    private Consultation consultation;
}

@Entity
@Data
@NoArgsConstructor
@AllArgsConstructor
public class Consultation {
    @Id
    private int id;
    private String description;
    private String traitementPrescrit;
    private String typeConsultation;
    @OneToOne
    private RendezVous rendezVous;
}
```

# b) Code des interfaces JPA Repository basées sur Spring Data:

```java
import org.springframework.data.jpa.repository.JpaRepository;

public interface PatientRepository extends JpaRepository<Patient, Integer> {
    List<Patient> findByNomContaining(String keyword);
}

public interface RendezVousRepository extends JpaRepository<RendezVous, Integer> {
    List<RendezVous> findByPatient(Patient patient);
}

public interface ConsultationRepository extends JpaRepository<Consultation, Integer> {
//
}
```

### Couche Métier

- Ecrire le code de l’interface `IHopitalMetier` permettant de répondre aux
spécifications fonctionnelles suivantes :
• Consulter les clients dont le nom contient un mot clé
• Consulter les rendez-vous d’un patient
- Ecrire le code java d’une implémentation de l’interface IHopitalMetier

# a) Code de l'interface IHopitalMetier :

```java
public interface IHopitalMetier {
    List<Patient> chercherPatientsParNom(String motCle);
    List<RendezVous> consulterRendezVousPatient(Patient patient);
}
```

# b) Code d'une implémentation de l'interface IHopitalMetier :

```java
@Service
public class HopitalMetierImpl implements IHopitalMetier {
    private PatientRepository patientRepository;
    private RendezVousRepository rendezVousRepository;

    public HopitalMetierImpl(PatientRepository patientRepository, RendezVousRepository rendezVousRepository) {
        this.patientRepository = patientRepository;
        this.rendezVousRepository = rendezVousRepository;
    }

    @Override
    public List<Patient> chercherPatientsParNom(String motCle) {
        return patientRepository.findByNomContaining(motCle);
    }

    @Override
    public List<RendezVous> consulterRendezVousPatient(Patient patient) {
        return rendezVousRepository.findByPatient(patient);
    }
}
```

### Couche Web

-  Ecrire le code du Contrôleur Spring MVC d’effectuer l’opération demandée

# a) Code du Contrôleur Spring MVC pour effectuer l'opération demandée :

```java
@Controller
public class PatientController {
    private IHopitalMetier hopitalMetier;

    public PatientController(IHopitalMetier hopitalMetier) {
        this.hopitalMetier = hopitalMetier;
    }

    @GetMapping("/patients")
    public String rechercherPatients(@RequestParam("motCle") String motCle, Model model) {
        List<Patient> patients = hopitalMetier.chercherPatientsParNom(motCle);
        model.addAttribute("patients", patients);
        return "liste-patients";
    }
}
```

### Sécurité


Pour sécuriser l'accès à l'application en se basant sur Spring Security avec un système d'authentification des utilisateurs et trois types de rôles (ROLE_PATIENT, ROLE_MEDECIN, ROLE_ADMIN), vous pouvez suivre les étapes suivantes :

a) Ajouter les dépendances Spring Security à votre projet Maven ou Gradle.

b) Configurer la classe `SecurityConfig` pour définir les règles de sécurité, les rôles et les autorisations.

```java
@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Autowired
    private PasswordEncoder passwordEncoder;
    
    @Bean
    public InMemoryUserDetailsManager inMemoryUserDetailsManager(){
        return new InMemoryUserDetailsManager(
                User.withUsername("patient").password(passwordEncoder.encode("1234")).roles("PATIENT").build(),
                User.withUsername("medecin").password(passwordEncoder.encode("1234")).roles("MEDECIN").build(),
                User.withUsername("admin").password(passwordEncoder.encode("1234")).roles("PATIENT","MEDECIN","ADMIN").build()


        );
    }
    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity httpSecurity)throws Exception{
        httpSecurity.formLogin().loginPage("/login").permitAll();
        httpSecurity.rememberMe();
        httpSecurity.authorizeHttpRequests().requestMatchers("/patient/**").hasRole("PATIENT");
        httpSecurity.authorizeHttpRequests().requestMatchers("/medecin/**").hasRole("MEDECIN");
        httpSecurity.authorizeHttpRequests().requestMatchers("/admin/**").hasRole("ADMIN");
        httpSecurity.authorizeHttpRequests().anyRequest().authenticated();
        httpSecurity.exceptionHandling().accessDeniedPage("/notAuthorized");
        return httpSecurity.build();

    }

}
```
