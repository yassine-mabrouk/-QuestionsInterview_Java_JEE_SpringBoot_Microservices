# Les Questions pour un entretien profile JAVA | JEE | Spring Ecosystem | Microservices 




## Partie 1: Questions java

- 1 . C'est quoi une classe Java? C’est une template définissant un type de données. Elle est utilisée pour créer des objets.

- 2 . Qu’est-ce qu’un objet? C’est un élément d’une classe (instance)

- 3 . Qu’es-ce qu’une méthode? C’est l’action qu’un objet peut faire.

- 4 . Heap vs Stack
  *  Heap: Lorsqu'un objet est créé, il est toujours créé dans Heap.
  *  Stack: Lorsqu'une fonction est appelée, un bloc est réservé en haut de Stack pour stocker ses variables locales. aussi on trouve les références aux objets qui sont utilisés par cette méthode.

- 5 . La différence entre JDK, JVM et JRE:
  *  JDK : Java Devlopment Kit. C’est l’ensemble des packages et programmes qu’on utilise pour écrire nos propres programmes.
  *  JRE : Java Runtime Environment . C’est la couche logicielle fournissant les packages et les ressources nécessaires pour qu’un programme java puisse s'exécuter.
  *  JVM : Java Virtuel Machine. C’est l’environnement dans lequel le code Java (Byte Code) s’exécute.

- 6 . Oracle JDK Vs OpenJDK
  * OpenJDK est une implémentation gratuite et open source de Java SE Platform Edition.
  * Oracle JDK nécessite une licence commerciale.

- 7 . Est-ce que Java utilise les pointeurs? Non, Java importe une couche de sécurité en utilisant les références à la place des pointeurs.

- 8 . les modificateurs d’accès en java: Ce sont les mots clés utilisés pour spécifier l’accès et la porté des objets,
  *  public : les classes, attributs, les méthodes peuvent être utilisés par n’importe quel objet.
  *  protected : Seules les classes du même packages ou des sous-classes qui peuvent utiliser les objets, attributs, méthodes avec ce modificateur.
  *  private: c’est le modificateur le plus restreint, les objets, attributs, méthodes, variables ne peuvent être utilisées que dans la classes où ils sont déclarés.
  *  « nothing » : pas de modificateur ou le modificateur par défaut, la visibilité est restreinte dans le même package.

- 9 . Quelle est la différence entre inner class et subclass?
  *  inner class : ou classe interne, est une classe définie (déclarée) à l’intérieur d’une classe.
  *  subclass : sous classe, est une classe fille d’une classe mère.

- 10 . Qu’est-ce qu’un constructeur? quels sont ses type?
Un constructeur est un bloc de code utilisé pour initialiser un objet. On distingue deux types de constructeur : constructeur par défaut, et constructeur paramètré.

- 11 . Overloading Vs Overriding?
  * Overloading : décrit le fait que deux méthodes (ou plus) peuvent avoir le même nom mais pas les mêmes parametres.
  * Overriding : décrit le fait que deux méthodes (ou plus) peuvent avoir le même nom et les mêmes parametres avec une relation mère-fille entre elles.

- 12 . Quelle est la différence entre equals() et ==?

== | equals() 
--- | --- 
Est un opérateur | Est une méthode
Pour la comparaison des primitives et des objets (leurs réferneces) |  Pour la comparaison de contenu des objets

- 13 . Qu'est-ce qu'un objet immuable ? 
Tu ne peux pas modifier les objets d'une classe immuable une fois qu'ils sont créés. (ex String)

- 23 . Quelle est la différence entre les classes String, StringBuilder et StringBuffer en Java ?

String | StringBuilder | StringBuffer
--- | --- | ---
String est une classe immuable. | Mutable | Mutable
... | non synchronisée  (not thread safe) | synchronisée  (thread safe)

- 14 . Différence entre Arraylist et List
  * List est une interface qui contient des méthodes abstraites. Une interface est un contrat qui doit être respecté par les développeurs.
  * ArrayList est une classe qui implémente l’interface List et respecte ce contrat. 

- 15 . C’est quoi le Garbage Collector?
C’est un mécanisme défini dans la JVM pour faire le ménage. Si un objet n’est plus utilisé, il sera automatiquement détruit pour libérer les ressources.

- 16 . Qu’est-ce qu’une exception?
C’est un problème qui se produit lors de l’exécution d’un programme, et qui nécessite un traitement spéciale pour le bon fonctionnement de l’application. Ceci peut être réalisé, soit par:
  *  l’envoi de l’exception à un niveau supérieur (throws) 
  *  ou par la capture et le traitement au niveau local (try/catch)

- 17 . Différence entre Exception et Error en java
  * Error représente les erreurs principalement causées par l’environnement d’exécution de l’application.
  * Exception représente les erreurs principalement causées par l’application elle-même. 
  
- 18 . C’est quoi une classe abstraite? 
 Est une classe qu'on peut pas l'instancier. Pour l’exploiter il faut absolument passer par l’héritage.
 
- 19 . C’est quoi une interface?
C’est une classe abstraite, qui permet de regrouper un certain nombre de méthodes sans qu’elle soit instanciée. Pour l’exploiter il faut l’implémenter

- 20 . Quelle est la différence entre une classe abstraite et une interface ?

Classe abstraite	 | Interface
--- | --- 
Les constructeurs sont autorisés	| Une interface ne peut pas avoir de constructeur.
Les méthodes static sont autorisées	| Les méthodes static ne sont pas autorisées
Une classe ne peut avoir qu'un seul parent abstrait | Une classe peut implémenter plusieurs interfaces
Une classe Java abstraite peut avoir des membres de classe private et protected | Les membres d'une interface Java sont public par défaut

- 21 . Différence entre une méthode statique et non statique

Méthode statique | Méthode non statique
--- | --- 
 appartient à une classe | appartient à un objet d’une classe. 
 ne peut accéder qu’aux membres statiques. |  peut accéder aux membres statiques et non statiques,

- 22 . Ordre d'execution d'un programme java:
static block -> Initialization block -> Constructor.

- 24 . size() vs length
La méthode size() fonctionne avec les collections, tandis que la propriété length fonctionne avec les tableaux.

- 25 . Quelles sont les étapes pour établir une connexion à une base de données?
  *  Enregistrer le driver
  *  Créer la connexion
  *  Créer le statement
  *  Exécuter la requête
  *  Récupérer les résultats ou l’état de l’exécution
  *  Fermer la connexion

---

## Partie 2: Questions générales JEE

- 1 . JEE : C'est l’ensemble de spécifications (JPA, JAX-WS, JMS...) pour créer des applications web Java, et c'est le serveur d’application qui fournit les implémentations.

- 2 . La version courante de la specification JEE est : Jakarta EE 9 (le 25 Mai 2021)

- 3 .	Les versions LTS Java sont : Java 8, 11, 17

- 4 .	AOP : La séparation des aspects métiers et des aspects techniques d'une application est rendu possible grâce à la programmation Orienté Aspect.

- 5 .	TDD : Test Driven Développement : développer d’abord les tests.

- 6 .	Statefull et Statless : Deux approches pour sécuriser application web.
  *  Statfull : la session de l’utilisateur authentifié est gérée par le serveur (avec état)
  *  Stateless : la session de l’utilisateur authentifié est gérée par le client.

- 7 .	Les méthodes Agile comme Scrum ou l'eXtreme Programming (XP) partent du constat que le cycle de développement en cascade est un échec.
  *  Des cycles de développement itératifs,
  *  L’implication du client final tout au long du projet,
  *  Des spécifications réduites en début de projet,

- 8 .	Maven est un outil permettant d'automatiser la gestion de projets Java. Il offre les fonctionalités suivantes: 
  *   Gérer les dépendances
  *   Lancer la compilation des sources
  *   Lancer les Test Unitaires
  *   Générer les packages (jar, war, ear)
  *   Installer les packages dans le repository 
  *   Déployer l’application dans le serveur 
  *   Générer la documentation du projet	

- 9 .	Lombok : une librairie java pour la génération de code automatique. Getter et setter …

- 10 .	DevTools : une librairie java vient avec spring boot, permet le rechargement automatiquement des classes Java et leur configuration côté serveur. Après les changements côté serveur, il s'est déployé dynamiquement,
---
## Partie 3: Spring framework 

- 11 . Spring : est un framework open source pour construire et définir l'infrastructure d'une application Java, dont il facilite le développement et les tests.

- 12 . Spring : est un framework de l’inversion contrôle pour créer des applications entreprises, on peut le sembler avec un conteneur web (tomcat) pour avoir un serveur application.

- 13 .	CotextLoaderListener est un listener appelé par Tomcat au moment du démarrage de l’application. Ce listener cherchera le fichier de beans spring. ce qui permet de faire l’injection des dépendances.

- 14 .	DispatcherServlet : Une Servlet qui joue le rôle de front contrôleur, pour traiter les requêtes de clients.

- 15 .	Differentes Configuration de Spring container :
  *  XML (ClassPathXmlAppContext(path xml file)
  *  Annotations (ClassPathXmlAppContext(path xml file)
  *  Code source Java (AnnotationConfigAppContext(ClassConfig.class)

- 16 .	Bean scope :
  *  Singleton ( scope par défaut )
  *  Prototype
  *  Request (Application web)
  *  Session (Application web)
  *  Global-session (Application web)

- 17 .	C'est quoi Spring container: 
  *  Création et gestion des beans (IOC)
  *  Injecter ces beans pour l’utiliser (DI)

- 18 .	Les types d’injection d’un Bean Spring:
  *  Via le constructeur (recommandé)
  *  Sous forme attribut avec l’annotation @Autoward

- 19 .	C’est quoi la differnec entre :
  *  @Param : Un parametre Spring Data
  *  @RequestParam : Un parametre Spring MVC, sous la forme ( url?variable=valeur ).
  *  @PathVariable : Un parametre Spring MVC, sous la forme ( url/varibale ).
  *  @PathParam : Un parametre Jersey
  *  @WebParam : Un parametre JAX-WS

- 20 .	Nouveautés de Spring 5 : Vient avec des fonctionnalités suivantes:
  *  Support de java 8 / 9
  *  Support de Hibernate 5 et Junit 5
  *  Support JPA 2
  *  Programmation fonctionnelle
  *  Support de kotlen
  *  Supprt de Http2

- 21 .	Spring boot : un module spring, ou une super couche de spring pour créer des applications spring avec zéro configuration.

- 22 .	Avantages spring boot :
  *  Auto configuration
  *  Serveur web intégré (Tomcat)
  *  Gestion de dépendances ( starters )
  *  Création des applications standalone (jar)

- 23 .	@SpringBootApplication : C'est une annotation de spring boot qui combine trois autres annotations:
  *  @Configuration: pour marquer une classe comme une classe de configuration,
  *  @EnableAutoConfiguration: pour activer la configuration automatique de spring boot.
  *  @ComponentScan: pour scanner les différentes classes constituant les Beans de notre application.

- 24 . Actuator: Une dépendance spring boot pour faire le monitoring de votre application en production.

- 25 . C'est quoi la différence entre @Controller et @RestController: Les deux servent à marquer une classe comme contrôleur, la différence est le type de retour, les méthodes de @Controller renvoient une vue HTML ou JSP, Tandis que celles de @RestController renvoient les données aux formats JSON, XML... ( @RestController = @Controller + @ResponseBody)


---

## Partie 4: Web service

- 1 .	Un API (Application Programming Interface) est un ensemble de règles : interfaces Annotations et des classes abstraites. permettent à votre produit ou service de communiquer avec d'autres produits et services sans connaître les détails de leur mise en œuvre.

- 2 .	Service web : C’est des composants web basés sur HTTP pour la communication et l'échange de données entre applications et systèmes distribués. On a deux spécifications  (JAX-WS et JAX-RS)

- 4 .	JAX-WS est une spécification JEE pour créer des web service basée sur le protocole SOAP, et interagit avec les messages XML.

- 3 .	JAX-RS est une spécification JEE pour créer des web service basée sur la norme Restful. et interagit avec les messages XML, JSON, HTML… 
(Implementations RESTEasy ET Jersey, Spring MVC, RestController, spring data rest).

- 5 .	Jersey est une implémentation de référence de JAX-RS.

- 6 .	SoapUI est une application de test de services web SOAP (Simple Object Access Protocol)  et  REST.

- 7 .	RESTful  ou REST : est un style architectural utilisé dans le développement de web services.

- 8 .	JMS est une spécification pour la communication asynchrone entre les applications.

- 9 .	KafKa : est un broker (provider)  pour le stockage ( file d’attente)  et l'échange  des messages entre les applications en mode asynchrone.

- 10 . WSDL (Web Service Description language) : un document XML qui contient la description de l’interface de web service.( méthodes de web service, paramètres d’entrée et sortie)

- 11 . UDDI (Universal Description Discovery and Integration) : Annuaire des web service permettant à la fois la publication (Register) et l’exploration (Discover) de web services.

- 12 . JAXB : Une librairie Java pour le mapping OXM objet / xml.  Ex(@XMLTransieint)

- 13 . XML : Format de données un peu lourd mais avec les schémas XSD on a la garantie que les données sont valides.

- 14 . JACKSON : Une librairie Java pour le mapping objet / JSON. Ex(@JsonIgnore)

- 15 . JSON : Format léger d’échange de données le plus recommandé. 

- 16 .	Projection : Citez les attributs d’une classe retournés par un service web.

- 17 .	Spécifications et implémentations

Spécification | Implémentation de référence (Oracle) | Autres implémentations 
--- | --- | --- 
JAX-WS | GlassFish Metro (Oracle) | CXF 
JAX-RS | Jersey (Oracle) | RestEasy(Jboss), SpringMVC 
JPA | Eclipselink (Oracle) | Hibernate (Jboss), Ibatis 
Serveur Application | Glassfish (Oracle) | Wildfly (Jboss), websphere(IBM) 
Bean validation | Hibernate Validation | Apache Bean Validation (formerly agimatec)


---
## Partie 5: Persistence de données ( JDBC, JPA, Hibernate, Spring data)

- 1 . JDBC (Java DataBase Connectivity) est une API fournie avec Java permettant de développer des applications capables de se connecter à des bases de données relationnelles (SGBDR).

- 2 .	JPA : Java persistence Api : C’est une spécification pour le mapping objet relationnel ORM, vient pour standariser différents framework ORM comme Hibernate, ExlepseLink.

- 3 .	Hibernate : le framework de mapping objet relationnel le plus populaire, c’est l’implémentation de JPA.

- 4 .	Avantages d'ORM :
  *  Code généré automatiquement
  *  Cache, performance
  *  HQL ou JPQL
  *  Indépendant de la base de données.

- 5 . Qu'est-ce que HQL ?
Hibernate Query Language (HQL) est utilisé comme une extension de SQL. HQL est la représentation orientée objet du langage de requête, c'est-à-dire qu'au lieu d'utiliser le nom de la table, nous utilisons le nom de la classe qui rend ce langage indépendant de toute base de données.

- 6 .	Spring data : Module de Spring, contient les interfaces et implémentations génériques qui utilisent JPA pour faire le mapping Objet Relationnel.

- 7 .	Quelques Annotations JPA: @Entity, @Id, @GeneratedValue, @Table, @Column, @Inheritance, @JoinColumn, @ManyToMany, @Transient

- 8 . Quelques contraintes sur une entité JPA : Une classe d'entité doit remplir les conditions suivantes :
  *  La classe doit avoir un constructeur sans parametres.
  *  La classe ne peut pas être "final".
  *  La classe doit être annotée avec l'annotation @Entity et @Id.
  
- 9 .	Cycle de vie d'une entité JPA : 
  *  Transient, [new()]
  *  Persistent, [save(), persist(), saveOrUpdate(), merge(), load(), get() ]
  *  Detached, [session.close(), session.clear(), session.evict(obj)]

- 10 . Quelle est la différence entre persist(), save(), merge() and update() ? 
  *  Vous pouvez utiliser les méthodes persist(), save() pour stocker une nouvelle entité (Transient) dans la base de données.
  *  Et merge(), update() pour enregistrer les modifications d'une entité détachée (Detached) dans la base de données.

- 11 .	Quelle est la différence entre load() et get()?
Lorsque l'objet n'est disponible ni dans le cache ni dans la base de données,
  *  load() : lève une exception (ObjectNotFoundException). la méthode load() peut retourner un proxy (lazy loading)
  *  get() : renvoie null. renvoie jamais de proxy, elle atteint toujours la base de données.
  
- 12 .	Différentes stratégies de Mapping d’héritage : @Inheritance(strategy= InheritanceType.SINGLE_TABLE)
  *  Une table par la hiérarchie : SINGLE_TABLE  (la plus utilisée) 
 		 @DiscriminatorColumn: Ajoutez cette annotation dans la classe mère, et @DiscriminatorValue dans les classes filles.
  *  Une table pour chaque classe concrète : TABLE_PER_CLASS
  *  Une table pour la classe mère et une table pour chaque classe fille: JOINED_TABLE

- 13 .	Les relations avec JPA et le fetch par défaut (JPA2+) :

Relation | fetch par defaut
--- | --- 
@OneToMany | LAZY
@ManyToMany | LAZY
@ManyToOne | EAGER
@OneToOne | EAGER

  *  FetchType.LAZY : indique que la relation doit être chargée à la demande ;
  *  FetchType.EAGER : indique que la relation doit être chargée en même temps que l'entité qui la porte.

- 14 .	Les niveaux de cache JPA : 
  *  L1 est activé par défaut, et réside dans l'objet de session d'hibernation. 
  *  L2 (cache hibernate) Ceci n'est pas activé par défaut. Il doit être configuré explicitement, et réside dans l'objet SessionFactory et de ce fait, les données sont accessibles par l'ensemble de l'application. parmi les implémentations on trouve ehcache (Easy Hibernate cache).

- 15 .	Transaction : Traiter un ensemble d’opérations comme une seule pour avoir des données cohérentes, pour gérer les transactions on utlise JTA (Java Transaction API),

- 16 .	Qu'est-ce qu'une session Hibernate ?
Une session est un objet qui maintient la connexion entre l'application objet Java et la base de données. Session a également des méthodes pour manipuler les données de la base de données à l'aide de méthodes telles que persist(), load(), get(), update(), delete(), etc.

- 17 .	Qu'est-ce qu'une SessionFactory ?
Est une classe qui permet de créer une instance de Session, afin d'établir la connexion à la base de données. Comme bonne pratique, l'application a généralement une seule instance de SessionFactory. 

- 18 . la différence entre les méthodes getCurrentSession et openSession ?
  *  getCurrentSession()	: Cette méthode renvoie la session liée au contexte. Cet objet de session est fermé une fois la SessionFactory est fermée.
  *  openSession() : Cette méthode ouvre toujours une nouvelle session. C'est le développeur qui va fermer cet objet une fois toutes les opérations de base de données terminées.

- 19 . Qu'est-ce qu'un Entitymanager ?
EntityManager est une API qui gère le cycle de vie des instances d'entité JPA.

- 20 . Les requêtes JPA :
  *  requêtes Natives.      entityManager.createNativeQuery(...)
  *  Requêtes JPQL.         entityManager.createQuery(...)
  *  l'API Criteria         entityManager.getCriteriaBuilder().createQuery(...) 

- 21 . Quelle est la différence entre JPA et JDO ?
  *  JPA (Java Persistence API) se concentre uniquement sur les bases de données relationnelles, 
  *  Alors JDO (Java Data Objects) est une spécification plus générale qui décrit l'ORM pour toutes les bases et référentiels possibles.


---
## Partie 6: Programmation Réactive en Java

- 1 . Deux modèles de programmation :
  * 	Modèle multi threads bloquant
    *  Programmation impérative.
    *  Basé sur un pool de threads.
    *  Les entrées sorties bloquants
  * 	Modèle single thread non bloquant 
    *  Programmation Réactive.
    *  IO selector thread et des workers
    *  Les entrées sorties non bloquants (NIO java 7).  
    *  Je dépends pas à la Tence des clients.

- 2 .	Nodjs : c’est la première téchnologie qui a introduit la programmation asynchrone en se basant sur le pattern Reactor.

- 3 .  Programmation Réactive : Modèle de programmation basé sur les événements en utilisant une séquence d’observables (Streams).

- 4 .	Streams : sont simplement les flux continues de données. Cela peut être n'importe quoi, des appels de service RESTful, des listes de données provenant d'une base de données, etc.

- 5 . Operations sur streams.
  * 	Intermediate operation: Renvoyer un nouveau flux sur lequel un traitement ultérieur peut être effectué.
    *  map(): produit un nouveau flux après avoir appliqué une fonction à chaque élément du flux d'origine. Le nouveau flux pourrait être de type différent.
    *  filter(): cela produit un nouveau flux qui contient des éléments du flux d'origine qui réussissent un test donné (spécifié par un prédicat).
  * 	Terminal operation: Marquer le flux comme consommé, après quoi il ne peut plus être utilisé.
    *  forEach(): il boucle sur les éléments du flux.
    *  collect(): nous collectons tous les éléments du flux dans une liste.

- 6 .	La différence entre Map et flatMap : 
  * 	Map : Transformer les objets d'un flux en un autre type d'objets.
  * 	FlatMap : FlatMap transforme chaque élément du flux en un flux d'autres objets.

- 7 . Deux API pour travailler avec la programmation réactive :
  * 	Reactive Streams : API pour développer des applications réactive, implementations: Reactor de Spring, Vertx de Java.
  * 	Reactive X : est une API pour développer des applications réactive, implementations (RxJs, RxJava)

- 8 .	Publisher: est celui qui va émettre les données

- 9 .	Subscriber : est celui qui va les recevoir en s’abonnant au Publisher.

- 10 .	Backpressure : c’est le subscriber qui va décider combien de données qu’il va recevoir.

- 11 .	L’échange de données entre Publisher et Subscribe va se terminer par :
  *  	Complete : si tout se passe bien
  * 	Error : si il ya un problème.

- 12 .	Reactor : Est la bibliothèque réactive de choix pour Spring. Se compose principalement de deux types de Stream.
  * 	Flux<T>: Un Publisher correspondant à un échange de 1 à plusieurs éléments.
  * 	Mono<T> : Un Publisher correspondant à un échange de 0 à 1 élément.

- 13 .	Spring webflux : est un projet spring introduit pour prendre en charge la programmation réactive dans le Web. C'est une alternative à Spring MVC qui est basée sur Servlet, Il a été introduit pour la première fois avec Spring 5. (spring-boot-starter-webflux)
	
- 14 . Pouvons-nous exécuter des applications Spring Webflux sur Tomcat ?
La seule exigence est que le serveur soit conforme à la spécification Servlet 3.1+. Cependant, les applications Spring Webflux sont généralement déployées sur des serveurs Web tels que Netty et Undertow.
	
- 15 .  Quel est le cas d'utilisation de Spring Webflux ?
Nous devrions l'utiliser lorsque nous voulons construire des systèmes qui sont résistants à une charge élevée. avec un nombre reduit de threads.

- 16 .	WebClient : Api qui permet d’accéder des services distants d’une manière réactive, est une alternative au classique RestTemplate.

---

## Partie 7: Micro-services

- 1 .	Deux architectures :
  *  Architecture basé sur une application monolithique 
  *  Architecture basé sur les micro-services.

- 2 .	Application monolithique : est une application qui est développée en un seul bloc ( jar, war )  avec une seule technologie. et déployée d’une manière unitaire dans un serveur d’application.

- 3 .	Problèmes d’une application monolithique : 
  *  Centralise tous les besoins fonctionnels
  *  Est réalisée dans une seule technologie. 
  *  Chaque modification nécessite la redéployèrent de toute application.
  *  Livraison en bloc, client attend beaucoup de temps pour commencer à voir les premières versions.

- 4 .	Les micro-services sont une approche d’architecture et de développement d’une application composée de petits services. L’idée étant de découper un grand problème en petites unités implémentée sous forme de micro-services.

- 5 .	Avantages d’une application basée sur micro-services
  *  Performances
  *  Redéploiement à chaud
  *  Technologies différentes
  *  Equipes indépendantes
  *  Facile à appliquer agilité et TDD

- 6 .	Désavantages d’une application basée sur micro-services
  *  la communication entre les méthodes est plus lente, 
  *  plus difficiles à déboguer.
  *  il y aura un effort supplémentaire pour les opérations, le déploiement, scaling, configuration, monitoring et les tests car chaque service est séparé.

- 7 . Les cas d'utilsation de l'architecture microservices: 
  *  Application très large.
  *  Besion de scaler l'application.
  *  Des grandes équipes.

- 8 .	Spring Cloud: Projet Spring pour créer des applications microservices, fournit registration, configuration et Proxy service.

- 9 .	Eureka Server ou service registry : Est un microservice technique qui enregistre la localisation des micro-services créer par Netflix :
  *  Nom de micro-service
  *  Adresse IP
  *  Port
  
  Pour l'implementer:
  *  ajouter la dépendance (spring-cloud-starter-netflix-eureka-server)
  *  ajouter cette annotation dans la classe main. @EnableEurekaServer	// Enable eureka server

- 10 .	Configuration service : Est un microservice qui centralise la configuration de tous les micro-services.

- 11 .	Proxy service : Dispatcher toutes les requêtes des clients vers les instances, donc il fait équilibrage de charge (load balancer)
  *  ZUUL : Est un proxy qui utilise un model multi threads avec IO bloquantes, [  @EnableZuulProxy		pour l'activer. sa dépendance (spring-cloud-starter-netflix-zuul)]
  *  Spring cloud Gateway : Est un proxy qui utilise un Model single threads avec IO Non bloquantes

- 12 . Circuit breakers: Est un design pattern qui permet d'éviter une défaillance sur le système. 

- 13 . Hystrix: C'est une implementation de Circuit breaker fournit par Netflix, qui donne un contrôle sur la latence et l'échec entre les services distribués. (spring-cloud-starter-hystrix)

- 14 . Spring Sleuth: est un outile qui va donner un ID unique à chaque requête à travers nos Microservices, de façon à pouvoir les suivre avec précision. (spring-cloud-starter-sleuth)

- 15 . Zipkin: Est une dépendence pour tracer et suivre des requêtes , C-à-d voir le chemin qu'une requête a parcouru afin de détecter où le problème s'est déclenché. (spring-cloud-sleuth-zipkin)

- 16 .	OpenFeign : Faire communiquer les micro-services distants en mode synchrone, et basé sur Ribbon pour faire l’équilibrage de charge.
       (spring-cloud-starter-openfeign)

- 17 . Pourquoi les conteneurs sont-ils utilisés dans les Microservices ? Parce que nous devons déployer beaucoup, et scaler notre microservice dans plusieurs machines.

- 18 . quelle est la signification de OAuth ?  un protocole d'autorisation permet à vos clients de créer un compte sur votre application web en se connectant sur un compte appartenant à une société vérifiée, comme Google, Facebook, Twitter, Okta ou GitHub...

- 19 .	C'est quoi Swagger ? un projet open source qui offre des outils permettant de générer la documentation pour les API Web. il respecte le standard OpenAPI, Il offre également une interface permettant d’explorer et tester les différentes méthodes offertes par ces services.

- 20 .	C'est quoi MapStruct ? Pour faire le mapping objet / objet ( DTO)

- 21 .	Quand est-we que on est besion de Base de données NoSql ? Quand la quantité de données est très importante, exemple MongoDb



