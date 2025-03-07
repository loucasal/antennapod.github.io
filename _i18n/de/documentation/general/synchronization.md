{% capture img-devices %} {% include image.html alt="

       Geräte

       "

loc="/assets/images/documentation" file="gpodder-devices.png" %} {% endcapture %}

{% capture img-synchronize %} {% include image.html alt="

       synchronisiere

       "

loc="/assets/images/documentation" file="gpodder-synchronize.png" %} {% endcapture %}

AntennaPod kann deine Abonnements und deinen Hörfortschritt mit anderen AntennaPod-Installationen sowie anderen (Desktop-)Anwendungen synchronisieren. Um die Synchronisierung einzurichten, benötigst du einen Server – den zentralen Punkt, über den deine Daten mit anderen Geräten geteilt werden. Hierfür hast du mehrere Möglichkeiten:

* [gpodder.net](https://gpodder.net/) bietet einen kostenlosen gPodder-Synchronisations-Server an, für den sich **jeder anmelden kann**. Leider ist dieser Server aufgrund der Beliebtheit des Dienstes und seiner begrenzten Finanzierung oft überlastet, was zu Fehlern in AntennaPod führt.
* Technisch versierteren Benutzern wird dringend empfohlen, **selbst einen Synchronisations-Server zu betreiben**. Ein selbst betriebener Server ist zuverlässiger und trägt dazu bei, die Belastung der kostenlosen öffentlichen Dienste zu verringern. Es gibt mehrere Optionen: [Nextcloud](https://nextcloud.com/install/#instructions-server) mit der [gPodder-Sync-App](https://apps.nextcloud.com/apps/gpoddersync), ein vollständiger [gPodder](https://gpoddernet.readthedocs.io/en/latest/dev/installation.html)-Server oder der [Micro-GPodder-Server](https://github.com/bohwaz/micro-gpodder-server).

## Synchronisierung per Nextcloud aktivieren

1. Wenn du ein Nextcloud-Konto hast, installiere die gPodder-Sync-App oder bitten deinen Server-Administrator, dies zu tun
1. Öffne `Einstellungen` » `Synchronisation` in AntennaPod und tippe auf `Anbieter für Synchronisierung auswählen`
1. Wähle „Nextcloud“
1. Gib die „Server-Adresse“ (die URL oder IP-Adresse des Servers) ein und tippe auf `Weiter zur Anmeldung`
1. Melde dich in dem sich öffnenden Browserfenster an und autorisiere AntennaPod

## Synchronisierung per gPodder aktivieren

1. Erstelle ein Konto auf gpodder.net oder melde dich an, solltest du bereits eines haben
1. When you have an account, log in on the webserver and create a device under `Subscriptions` » `Devices` for each client that you use:<br />{{ img-devices | strip }}
1. When you have added the devices to your account, link them using the "Configure" button. This way, gpodder.net automatically keeps the activated devices synchronized.<br />{{ img-synchronize | strip }}
1. Öffne `Einstellungen` » `Synchronisation` in AntennaPod und tippe auf `Anbieter für Synchronisierung auswählen`
1. Wähle „gPodder“
1. Gib die „Server-Adresse“ (z. B. www.gpodder.net) ein und tippe auf `Weiter zur Anmeldung`
1. Gib den „Benutzernamen“ und das „Passwort“ ein und tippe auf `Anmelden`
1. Wähle das Gerät aus, das du auf dem Server erstellt hast

**Anmerkung:** Hast du ein Gerät während der Einrichtung der Synchronisierung erstellt und nicht davor, wie oben beschrieben? Dann stelle sicher, dass du auf die Schaltfläche `Komplette Synchronisation erzwingen` in AntennaPod tippst, um den Abspielstatus aller Episoden hochzuladen, die du zuvor angehört hast. Wenn du dies nicht machst, werden nur Podcasts synchronisiert, die **nach** der Verknüpfung der Geräte hinzugefügt wurden. Es gibt ein [offenes Issue für gpodder.net](https://github.com/gpodder/mygpo/issues/388), das darum bittet, dieses Verhalten zu ändern.
