# Hibernate and JPA Projects

Collection of Java persistence exercises covering project management, civil-status records, and stock management.

## What Is Demonstrated

- Direct Hibernate configuration through project-specific `HibernateUtil` classes
- Entity inheritance in the civil-status domain
- Join entities for project-task and stock-order relationships
- Generic DAO interfaces and service layers
- PostgreSQL-oriented configuration and Docker Compose material

## Modules

| Module | Domain |
| --- | --- |
| `gestion_de_projets` | Projects, employees, and tasks |
| `gestion_de_etat_civil` | Civil-status records |
| `gestion_de_stock` | Products, categories, orders, and order lines |

Each module contains its own Maven configuration, entities, DAO interfaces, services, and executable test classes.
