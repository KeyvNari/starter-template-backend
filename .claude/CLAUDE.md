This app is a full stack agents platform, to let users use chatbots or different AI services.


When adding new model and its api cruds always keep in mind that:

1. The services for each model should be created in app/services
2. Stay conformal on how other services interact with the db
3. Model are defined in /root/full_stack_agents_platform/backend/app/models
4. Make sure to import the new models in app/models/__init__.py
5. You can run the alembic migrations using uv, for example: uv run alembic revision --autogenerate -m "Add new model"

The api routes are defined in app/routes
Make sure to add new routes to app/routes/__init__.py