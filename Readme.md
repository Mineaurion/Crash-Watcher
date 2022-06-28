# Crash Watcher

Notify on discord channel when a crash-reports file is created.

## Getting Started

Install the crash-watcher.service at `/etc/systemd/system` and put the crash-watcher into `/usr/local/bin/`. The sh file must be executable in case it's not, use this command :

```sh
chmod +x /usr/local/bin/crash-watcher.sh
```

Before launching the service you need to add the ini file and custom the settings.

```sh
cp crash-watcher.example.ini /etc/crash-watcher.ini
```

And after you just have to start the service and you are good to go.

### Prerequisites

You need to have inotify-tools and jq installed on the machine.

```sh
sudo apt install inotify-tools jq
```

You need to create an user key from the pterodactyl panel, once you created it you can edit the ini file to add it.
