# Alarms, Reminders, and Timers Management
This Home Assistant blueprint, **View Assist – Alarms Reminders Timers**, allows users to set, manage, and cancel alarms, reminders, and timers using voice commands.  
It integrates with Home Assistant’s conversation platform and provides customizable sentences for seamless voice interactions.  
The blueprint also supports multiple languages (e.g., English, German, French, Spanish) and can show active alarms, reminders, or timers on a dashboard if a compatible device is available.  
Some translations were automatically generated and may benefit from refinement — feel free to submit a PR for improvements!

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fdinki%2FView-Assist%2Frefs%2Fheads%2Fviewassist-integrationprep%2FView_Assist_custom_sentences%2FAlarms_Reminders_Timers%2Fblueprint-alarmsreminderstimers.yaml)

## Example Sentences
- "Set a timer for 5 minutes."
- "Remind me to take out the trash at 8 PM."
- "Set an alarm for 7 AM."
- "How much time is left on my timer?"
- "Cancel my reminder."
- "Show my alarms."

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

## TODO
- [ ] Add new view to list timers, alarms, and reminders (dedicated, instead of current info view)
- [ ] Update backend to handle shorten versions of time (e.g. "5m" instead of "5 minutes")
- [ ] Add support for more languages in backend (mainly for the 'text' attribute of the timer)
