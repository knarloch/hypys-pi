# hypys-pi
Private raspberry pi tweaks and configuration notes

## raspotify
Standard raspotify package supports systemd, this is sysvinit init.d script based on
https://gist.github.com/chojnac/496f1716fb12af848871c5b5eeffc5ec .
It has been updated to take into account pulseaudio configuration:

* added dependency to pulseaudio
* added a note with correct groups configuration for raspotify user
* modified piddir

After installing, run `update-rc.d raspotify defaults`
