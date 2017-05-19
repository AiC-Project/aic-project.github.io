---
layout: default
title: {{ site.name }}
lang: fr
langTitle: Français
ref: home
---

## Améliorer la qualité et les coûts du développement Android

AiC 2.0 a pour objectif de faciliter la qualification à grande échelle des applications Android.

Techniquement il s’agit de proposer une réponse à la multiplication des terminaux physiques (smartphones, tablettes, TV connectées) et des versions du système d’exploitation Android, à travers une solution Cloud complète et simple d’utilisation.

Cette solution repose fortement sur la mise à disposition de machines virtuelles Android.

L’avantage de cette approche est d’accélérer les temps de déploiement et de configuration des environnements de test Android, tout en réduisant considérablement l’investissement et la maintenance d'un parc de périphériques physiques.

## Effectuer des tests Android manuels ou automatisés

La solution Saas AiC 2.0 présente à son utilisateur deux grandes fonctionnalités : la campagne "live" et la campagne asynchrone.

### Campagne "live"

Grâce à la campagne "live", vous pouvez interagir avec une instance virtuelle Android depuis l'interface web AiC 2.0, directement dans votre navigateur, sans plugins supplémentaires.

![AiC Live Campaign](/img/AiC_live_campaign_640.gif){:class="img-responsive"}

__En quelques mots, _c'est Android dans le navigateur.___

Parmis les fonctionnalités de la campagne live :

- choix de la version Android (téléphone ou tablette, KitKat ou Lollipop)
- configuration de la résolution et de la densité de pixels
- installation des apks en temps réel
- stimulation des capteurs Android depuis l'interface web (dont GSM et Wifi)
- possibilité de passer en plein écran ou d'adapter la vue à la taille de votre écran

### Campagne asynchrone

Grâce à la campagne asynchrone, vous pouvez programmer une campagne qui éxécutera vos tests UiAutomator ou AiC 2.0 à grande échelle sur un parc d'instances virtuelles Android configurables. Les instances virtuelles sont accessibles visuellement durant l'exécution du jeu de tests, et les résultats sont ensuite présentés au format Junit. 

![AiC Async Campaign](/img/AiC_async_campaign_640.gif){:class="img-responsive"}

__En quelques mots, _c'est Android dans le Cloud.___

Parmis les fonctionnalités de la campagne asynchrone :

- possibilité d'utiliser les tests natifs UiAutomator ou le DSL dédié AiC 2.0
- choix des versions d'Android sur lesquelles exécuter les tests
- notifications en temps réel de l'état d'avancement de la campagne
- instances virtuelles accessibles durant l'exécution des tests
- résultats des campagnes sauvegardés et présentés au format Junit

### Le DSL AiC 2.0
Le DSL AiC 2.0 est une innovation spécifique au projet permettant à un utilisateur d'exprimer un test fonctionnel en langage naturel proche de Gherkin. Par rapport aux solutions de tests classique Android (UiAutomator, Espresso, Junit), le DSL AiC 2.0 permet d'exprimer des tests fonctionnels tout en précisant l'état des senseurs système (dont Bluetooth, NFC).

{% highlight gherkin%}
Feature: "Example feature"

    Scenario: "Minimal example scenario"
        Set battery level at 5
        Check if "Low battery" exists
    End

    Scenario: "More complex example scenario"
        Click on “Sensor”
        Scroll from "Picture" to "Photometer"
        Scroll from "Photometer" to "Gyroscope
        Click on "Proximity Sensor"
        Type "Value is going to change..." into "R.id.input_exemple"
        Set sensor "TYPE_PROXIMITY" at 18
        Replace "It's working !" into "R.id.input_exemple"
        Click on "Proximity Sensor"
        Scroll from "Proximity Sensor" to "Bluetooth"
        Click on "Ambient Thermometer"
    End

End
{% endhighlight %}


En résumé, le DSL AiC 2.0 permet de :

- exprimer des tests fonctionnels Android en langage naturel type Gherkin
- décrire l'état du système Android dynamiquement dans la séquence de test
- compiler un apk de test utilisable ensuite en campagne asynchrone

## Utiliser la solution AiC 2.0

Deux possibilités s'offrent à vous pour utiliser AiC 2.0 :

- demander un accès à la version hébergée sur le testbed FIT UPMC Cloud Openstack. Accessible ici : [AiC 2.0](https://aic.onelab.eu:8443/). L'accès est gratuit mais requiert [une inscription au portail Onelab](https://portal.onelab.eu/register).

- installer la solution depuis les sources [Github](https://github.com/AiC-Project)



There are two ways to use AiC 2.0 :
You can use beta version hosted on FIT UPMC Cloud Openstack testbed. You can access it here:  AiC 2.0, it is free of charge, but you will need to create OneLab account. 
install the solution from the Github sources

## Consortium et financement

### Les partenaires à l'origine du projet
Le consortium du projet AiC 2.0 réunit les partenaires industriels et académiques suivants : 

- Alter Way, partenaire industriel et pilote du projet
- Zenika, partenaire industriel
- Liafa, partenaire académique
- Lip6, partenaire académique
- Thalès, grand utilisateur

![AiC Partners Logo](/img/AiC_partners_logo.png){:class="img-responsive"}

### Le cadre de financement
Le projet AiC 2.0 est un projet de R&D collaboratif issu de l’appel à projets [FUI#16](http://www.systematic-paris-region.org/fr/actualites/le-16e-appel-a-projets-fui-retient-12-projets-labellises-par-systematic-paris-region). 

Le FUI (pour Fonds Unifiés Interministériel) est un programme destiné à soutenir la recherche appliquée, pour aider au développement de nouveaux produits et services susceptibles d'être mis sur le marché à court ou moyen terme.

Il permet de financer les projets de R&D dits « collaboratifs » (associant par exemple de grandes entreprises, des PME et des laboratoires), suite à leur labellisation par les pôles de compétitivité.

Le financement est ensuite géré par la BPI en association avec les collectivités, pour le projet AiC 2.0, la région Ile de France.

![AiC Financial Logo](/img/AiC_financial_logo.png){:class="img-responsive"}

### Engagement Open Source
Le code réalisé dans le cadre projet sera reversé sous licence Open Source, conformément à [la charte du GTLL](http://www.systematic-paris-region.org/fr/logiciel-libre/propos/charte).

### Calendrier du programme FUI
Démarré en Décembre 2013, le programme du projet est en cours et se concluera en Octobre 2017.


