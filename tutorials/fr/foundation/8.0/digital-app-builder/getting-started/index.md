---
layout: tutorial
title: Mise en route
weight: 3
show_children: true
---
<!-- NLS_CHARSET=UTF-8 -->
## Présentation
{: #getting-started }

Vous pouvez lancer Digital App Builder comme suit :

* Sous **MacOS**, cliquez deux fois sur l'**icône IBM Digital App Builder** pour ouvrir Digital App Builder.
* Sous **Windows**, lancez Digital App Builder en sélectionnant **Démarrer > Programmes > IBM Digital App Builder**.

>**Remarque** : Si vous ouvrez Digital App Builder pour la première fois, cliquez sur **Accepter** pour accepter la **Licence d'utilisation d'IBM Digital App Builder** dans l'écran clignotant pour continuer. Une fois que vous avez accepté le contrat de licence, la **Vérification des prérequis** s'exécute automatiquement pour la première fois. En l'absence d'erreurs, cliquez sur **OK** pour continuer ; sinon, corrigez les erreurs et redémarrez Digital App Builder.

![IBM Digital App Builder](dab-home-screen.png)

Vous pouvez **Créer une application**, **Ouvrir une application** ou utiliser les modèles disponibles pour générer votre application.
>**Remarque** : Vous pouvez voir vos applications récemment créées sous la section **Récent**. Dans le cas d'une nouvelle installation, la section **Récent** n'apparaît pas.


### Créer une application
{: #create-new-app }

Vous pouvez créer une application en cliquant sur l'icône **Créer une application** dans le tableau de bord de Builder.

1. Cliquez sur l'icône **Créer une application**. La fenêtre **Sélectionnez un canal** s'affiche.

    ![Sélectionnez un canal](dab-select-channel.png)

2. Sélectionnez le canal pour lequel vous souhaitez développer l'application en cliquant sur l'icône associée. Vous pourrez ajouter d'autres canaux à la même application ultérieurement.

    * **Android** : sélectionnez cette option si vous créez une application Android.
    * **iOS** : sélectionnez cette option si vous créez une application iOS.
        >**Remarque** : Vous pouvez générer et exécuter les applications iOS uniquement sur MacOS.
    * **Web** : sélectionnez cette option si vous créez une application pour le Web.
    * **PWA** : sélectionnez cette option si vous créez une application Progressive Web App.

3. La fenêtre **Sélectionnez le type de serveur auquel se connecter** apparaît.

    ![Sélectionnez le type de serveur auquel se connecter](dab-select-server.png)

4. Vous pouvez sélectionner un **Serveur Playground partagé** ou un **Serveur Professional personnalisé**.

    * **Serveur Playground partagé** : serveur Mobile Foundation partagé hébergé sur IBM Cloud pour démarrer rapidement.

        >**Avertissement** : Le serveur Playground partagé est un serveur commun partagé entre de nombreux développeurs. Il ne doit pas être utilisé pour des applications de production. Il n'est pas possible de supprimer les données de ce serveur sans notification. Le temps de disponibilité du serveur n'est pas garanti.

        ![Serveur partagé IBM](dab-shared-server.png)

        * Entrez la **Clé d'API IBM Cloud**. Pour plus d'informations sur les détails d'accès, voir [**Comment créer une clé d'API de plateforme ?**](../faq/) dans la rubrique Foire aux questions. 

        * Cliquez sur **Se connecter** pour vous connecter au serveur. 

    * **Serveur Professional personnalisé** : vous pouvez vous connecter à votre propre serveur Mobile Foundation créé sur IBM Cloud ou en local. La fenêtre **Configurer l'instance IBM Mobile Foundation** vous permet de sélectionner un serveur existant ou d'en créer un nouveau.

        ![Configurer l'instance IBM Mobile Foundation](dab-config-ibm-cloud-instance.png)
 
        La fenêtre **Configurer l'instance IBM Mobile Foundation** affiche la liste des instances de serveur Mobile Foundation que vous avez définies précédemment. Lors de la sélection du serveur, les options **Nom du serveur**, **URL du serveur**, **Nom d'utilisateur de l'administrateur** et **Mot de passe de l'administrateur** s'affichent. Pour définir un nouveau serveur, vous pouvez cliquer sur le lien **Créer un serveur**. La nouvelle fenêtre **Configurer l'instance IBM Mobile Foundation** s'ouvre.

        ![Créer un serveur](dab-custom-professional-server.png)

        * Entrez les détails de la nouvelle instance IBM Mobile Foundation : **Nom du serveur**, **URL du serveur**, **Nom d'utilisateur de l'administrateur** et **Mot de passe de l'administrateur**.
            >**Remarque** : Vous pouvez obtenir l'URL et les données d'identification de connexion du serveur dans le tableau de bord Mobile Foundation de l'instance de serveur sélectionnée.
        * Si vous le souhaitez, indiquez un **Nom d'utilisateur** (nom d'utilisateur du client confidentiel) et un **Mot de passe de l'administrateur** pour prévisualiser les données dans le visualiseur de données.
        * Cliquez sur **Se connecter**.

5. Une fois la connexion établie, la fenêtre **Créer une application** s'ouvre et vous permet de sélectionner une définition d'application existante que vous avez créée ou d'en créer une nouvelle en indiquant les détails appropriés. 
    * Dans le cas d'une nouvelle application, indiquez le **Nom** de l'application, l'**Emplacement** de stockage des fichiers de projet, le **Projet/ID de bundle** et la **Version** de l'application. 
 
        ![Serveur Playground partagé](dab-create-app.png)

    * Cliquez sur **Créer** pour créer l'application. La fenêtre **Bienvenue dans le plan de travail** s'affiche.
    * Cliquez sur **C'est parti !**. L'espace de travail de Digital App Builder s'ouvre pour vous permettre de créer une application ou d'en modifier une existante.

        ![Espace de travail DAB](dab-workbench.png)

### Ouvrir une application existante
{: #open-an-existing-app }
 
>**Remarque** : Vous ne pouvez ouvrir qu'une application existante développée avec Digital App Builder.

Vous pouvez ouvrir une application existante en procédant de l'une des manières suivantes :

* Cliquez sur **Ouvrir une application** dans la page d'accueil pour ouvrir l'explorateur de fichiers. Accédez au dossier de projet de l'application et cliquez sur **OK** pour ouvrir l'application et continuer à la modifier.
* Si vous le souhaitez, vous pouvez ouvrir l'application à partir de la liste des applications récentes, le cas échéant, en cliquant deux fois sur son nom.

### Utilisation de modèles
{: #using-templates }

Vous pouvez utiliser des modèles pour générer rapidement votre application. Il existe des modèles d'application activés pour des fonctionnalités spécifiques qui vous permettent de modifier et développer rapidement des applications. Seul l'agent conversationnel Watson est disponible à l'heure actuelle.
