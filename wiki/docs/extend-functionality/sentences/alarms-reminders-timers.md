---
title: Alarms Reminders & Timers
---

# Alarms Reminders & Timers

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fdinki%2FView-Assist%2Frefs%2Fheads%2Fmain%2FView_Assist_custom_sentences%2FAlarms_Reminders_Timers%2Fblueprint-alarmsreminderstimers.yaml)


Detailed install video: Coming Soon!

### Description
This custom sentence allows for an on demand call to create and list alarms, reminders and timers.  While this intial version is fully functional,  I do not take any responsibility if this makes you late for work, forget to buy your wife flowers, or if your eggs get overcooked.  There's your warning and my escape clause!


### Usage
Use your wakeword and say things like:

* Set a timer for 2 minutes
* Start an egg time for 3 minutes
* List my timers
* Remind me to wash the dog at 3pm
* Set a reminder to take the food out of the over in 30 minutes
* Cancel my egg timer
* Set an alarm for 4pm

### Requirements
- **View**:  [Alarm view](../views/alarm)

### Installation

* Find and upload a sound to play when the timer expires.  Need help?  See the Stream Assist video where I discuss how to find these and where to upload
* Install blueprint using button above and configure options

## Translations
This section provides examples of the custom sentences in different languages.  
Adjustments may be needed based on your specific usage and preferences.

### English
```yaml
sentences_set_timer:
  - set [a] timer for {when}
  - set [a] {when} timer
  - (set|start) [a|an] {name} timer for {when}
sentences_set_reminder:
  - (remind me | set a reminder) to {name} at {when}
  - remind me to {name} in {when} | set a reminder to {name} in {when}
  - remind me in {when} to {name}
sentences_set_alarm:
  - Set [an] alarm for {when}
  - Set [an] {name} alarm for {when}
sentences_cancel_timer:
  - cancel [my] {name} timer
  - stop [my] {name} timer
  - cancel [my] timer
  - stop [my] timer
sentences_cancel_alarm:
  - cancel [my] {name} alarm
  - stop [my] {name} alarm
  - cancel [my] alarm
  - stop [my] alarm
sentences_cancel_reminder:
  - cancel [my] {name} reminder
  - stop [my] {name} reminder
  - cancel [my] reminder
  - stop [my] reminder
sentences_list_timers:
  - (list|show|get) my timers
  - (list|show|get) my timer
  - what timers are set
  - what timers do I have
sentences_list_alarms:
  - (list|show|get) my alarms
  - (list|show|get) my alarm
  - what alarms are set
  - what alarms do I have
sentences_list_reminders:
  - (list|show|get) my reminders
  - (list|show|get) my reminder
  - what reminders are set
  - what reminders do I have
sentences_turnoff_alarm:
  - (Turn off | cancel | stop | snooze) alarm
sentences_time_remaining:
  - how much time (is) left on my {name} timer
  - how much time (is) left on my timer
```

### German
```yaml
sentences_set_timer:
  - Stelle einen Timer für {when}
  - Starte einen {when} Timer
  - (Stelle|Starte) einen {name} Timer für {when}
sentences_set_reminder:
  - (Erinnere mich | Setze eine Erinnerung) an {name} um {when}
  - Erinnere mich daran {name} in {when} zu tun
sentences_set_alarm:
  - Stelle einen Alarm für {when}
  - Stelle einen {name} Alarm für {when}
sentences_cancel_timer:
  - (Lösche | Stoppe) meinen {name} Timer
  - (Lösche | Stoppe) meinen Timer
  - Timer (stoppen | abbrechen)
  - Timer {name} (stoppen | abbrechen)
sentences_cancel_alarm:
  - (Lösche | Stoppe) meinen {name} Alarm
  - (Lösche | Stoppe) meinen Alarm
  - Alarm (stoppen | abbrechen)
  - Alarm {name} (stoppen | abbrechen)
sentences_cancel_reminder:
  - (Lösche | Stoppe) meine {name} Erinnerung
  - (Lösche | Stoppe) meine Erinnerung
  - Erinnerung (stoppen | abbrechen)
  - Erinnerung {name} (stoppen | abbrechen)
sentences_list_timers:
  - (Liste|Zeige|Zeig) meine Timer
  - Welche Timer sind eingestellt
  - Welche Timer sind gestellt
sentences_list_alarms:
  - (Liste|Zeige|Zeig) meine Alarme
  - Welche Alarme sind eingestellt
  - Welche Alarme sind gestellt
sentences_list_reminders:
  - (Liste|Zeige) meine Erinnerungen
  - Welche Erinnerungen sind eingestellt
  - Welche Erinnerungen sind gestellt
sentences_turnoff_alarm:
  - Alarm (ausschalten | stoppen | abbrechen | aus)
  - Timer (ausschalten | stoppen | abbrechen | aus)
sentences_time_remaining:
  - Wie viel Zeit (bleibt | ist ) auf meinem {name} Timer
  - Wie viel Zeit (bleibt | ist ) auf meinem Timer
```

### Spanish
```yaml
sentences_set_timer:
  - pon un temporizador de {when}
  - inicia un temporizador de {when}
sentences_set_reminder:
  - (recuérdame | establece un recordatorio) para {name} a las {when}
sentences_set_alarm:
  - Pon una alarma para {when}
  - Pon una alarma {name} para {when}
sentences_cancel_timer:
  - cancela [mi] temporizador {name}
  - detén [mi] temporizador
sentences_cancel_alarm:
  - cancela [mi] alarma {name}
  - detén [mi] alarma
sentences_cancel_reminder:
  - cancela [mi] recordatorio {name}
  - detén [mi] recordatorio
sentences_list_timers:
  - (lista|muestra|obtén) mis temporizadores
sentences_list_alarms:
  - (lista|muestra|obtén) mis alarmas
sentences_list_reminders:
  - (lista|muestra|obtén) mis recordatorios
sentences_turnoff_alarm:
  - (apaga | cancela | detén | pospone) alarma
sentences_time_remaining:
  - cuánto tiempo queda en mi {name} temporizador
  - cuánto tiempo queda en mi temporizador
```

### French
```yaml
sentences_set_timer:
  - règle un minuteur pour {when}
  - démarre un minuteur de {when}
sentences_set_reminder:
  - (rappelle-moi | configure un rappel) pour {name} à {when}
sentences_set_alarm:
  - règle une alarme pour {when}
  - règle une alarme {name} pour {when}
sentences_cancel_timer:
  - annule [mon] minuteur {name}
  - arrête [mon] minuteur
sentences_cancel_alarm:
  - annule [mon] alarme {name}
  - arrête [mon] alarme
sentences_cancel_reminder:
  - annule [mon] rappel {name}
  - arrête [mon] rappel
sentences_list_timers:
  - (liste | montre | obtiens) mes minuteurs
sentences_list_alarms:
  - (liste | montre | obtiens) mes alarmes
sentences_list_reminders:
  - (liste | montre | obtiens) mes rappels
sentences_turnoff_alarm:
  - (éteindre | annuler | arrêter | reporter) l'alarme
sentences_time_remaining:
  - combien de temps reste-t-il sur mon {name} minuteur
  - combien de temps reste-t-il sur mon minuteur
```

## Changelog

| Version | Description                                                                                                                                                          |
|---------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| v 1.1.0 | Added translations, adjusted behavior to handle timers, reminders and alarms, added option to run actions before warning is triggered (e.g. to wakeup device screen) |
| v 1.0.0 | Initial release                                                                                                                                                      |
