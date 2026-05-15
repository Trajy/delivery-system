COMPOSE_FILES = \
	-f docker-compose.yml \
	-f docker-compose.database.yml

PROJECT_NAME = delivery-system

up:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) up

down:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) down

restart:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) restart

build:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) build

logs:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) logs -f

ps:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) ps

pull:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) pull

destroy:
	docker compose $(COMPOSE_FILES) -p $(PROJECT_NAME) down -v --remove-orphans