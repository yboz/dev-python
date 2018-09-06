# dev-python
dev image for python apps

```
docker run -d --rm --net fluent-forward --name app \
				   -v /tmp/.X11-unix:/tmp/.X11-unix \
				   -v /var/run/dbus:/var/run/dbus \
				   -v /home/ybozkurt/.java/.userPrefs/:/home/dev/.java/.userPrefs/ \
				   -v /home/ybozkurt/.PyCharmCE2018.2/:/home/dev/.PyCharmCE2018.2/ \
				   -v /home/ybozkurt/tools:/home/dev/tools/ \
				   -v /home/ybozkurt/src:/home/dev/src/ \
				   -e DISPLAY=unix$DISPLAY \
				   graphical-python:3.5 \
				   /home/dev/tools/pycharm-community-2018.2.2/bin/pycharm.sh
```
