# toggl-notifier
* Update your Adium status with the description of your current task in Toggl
* Only for MacOS X

# Installation
* install the required libraries

        gem install rest-client json

* copy the required files

        mkdir ~/.toggl-notifier && \
        git clone git://github.com/crohr/toggl-notifier.git ~/.toggl-notifier && \
        chmod 600 ~/.toggl-notifier/config.yml && \
        chmod +x ~/.toggl-notifier/toggl-notifier

* Update `~/.toggl-notifier/config.yml` with your Toggl credentials
* Add an entry to your crontab:

        crontab -e

  and enter a new line with something like:

        */5 * * * * ~/.toggl-notifier/toggl-notifier

# References
* http://www.toggl.com

# Todo
* Package it as an Adium Script
