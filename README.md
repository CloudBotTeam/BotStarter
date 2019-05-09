# BotStarter
The starter of the project, you should read this before you start using or contribute to our project.

## QuickStart

### dev 

If you develop the app in your local machine, then you should:

```bash
mkdir CloudBotTeam
```

This will be your base project. Now you should clone all neccessary packages and submodules for our project:

```bash
git clone --recurse-submodules git@github.com:CloudBotTeam/service-manager.git
git clone --recurse-submodules git@github.com:CloudBotTeam/bot-manager.git
# git clone --recurse-submodules git@github.com:CloudBotTeam/CloudBot-Common.git
git clone git@github.com:CloudBotTeam/CloudBot-Service-Discovery.git
git clone git@github.com:CloudBotTeam/config-server.git
git clone git@github.com:CloudBotTeam/QQ-Bot.git
git clone git@github.com:CloudBotTeam/CloudGateway.git
```

Oh, you should also clone this repo ：）

```bash
git clone https://github.com/CloudBotTeam/BotStarter
```

Use this to build all Java packages:

```bash
mvn clean package dockerfile:build -DskipTests=true
```

And for QQ-Bot, you should just build a image called: `cloudbot/docker-api`

Then you should run 

```bash
docker-compose up
```

To build the project.

There is one thing you should remember: You'd better set more memory and CPU for docker, I use:

| config |  value  |
| :----: | :-----: |
|  CPUs  |    6    |
| Memory | 8.0 GiB |
|  Swap  | 1.5 GiB |

## Architechture

![arch](https://nmsl.maplewish.cn/1EF0AC2A-3162-4482-82E7-10F663CA43A4.png)

