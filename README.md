https://docs.google.com/document/d/1qZqo5S2m-cdaJu1nJ1KDR2QsSxg-4EIIAZ2Ek2g9ibE/edit?tab=t.0

Documentation


en raspberry

sudo docker run -d \
  --name amqp-broker \
  -p 5672:5672 \
  -p 15672:15672 \
  -p 1883:1883 \
  rabbitmq:3-management



python -m venv .venv
source .venv/bin/activate
pip install pika

sudo systemctl stop mosquitto
sudo systemctl disable mosquitto


----------la primera vez-----------
sudo docker run -d   --name amqp-broker   -p 5672:5672   -p 15672:15672   -p 1883:1883   rabbitmq:3-management


sudo docker exec amqp-broker rabbitmq-plugins enable rabbitmq_mqtt

----------------------------------la segunda vez---
sudo docker start amqp-broker
