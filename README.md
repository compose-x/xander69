### Helping xander out


#### Install

```shell
python3 -m venv venv
source venv/bin/activate
pip install pip -U
# Temporary until 0.23.0
pip install git+https://github.com/compose-x/ecs_composex@refactor/resources-and-stacks

```

#### Deploy

With the venv still activated

```shell
git clone https://github.com/compose-x/xander69
cd xander69
ecs-compose-x render -d templates -p osticket-app -f docker-compose.yaml -f aws.yaml
```

Change `render` with `up` or `plan` to deploy to AWS.
