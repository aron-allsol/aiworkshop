# AI Workshop - OpenEdge ABL Project

This project demonstrates modern OpenEdge ABL development patterns including:

- **Business Entity Architecture** - Layered architecture separating UI from business logic
- **Singleton Factory Pattern** - Centralized entity lifecycle management
- **Dataset-based Data Access** - Temp-tables and datasets for data transfer
- **Change Tracking** - BEFORE-TABLE pattern for update detection

## Project Structure

```
src/
  business/
    CustomerDataset.i    - Customer temp-table and dataset definition
    CustomerEntity.cls   - Customer business entity
    ItemDataset.i        - Item temp-table and dataset definition
    ItemEntity.cls       - Item business entity
    EntityFactory.cls    - Singleton factory for entity management
  CustomerWin.w          - Customer management window
  ItemWin.w              - Item management window
doc/
  business-entity-pattern.md - Architecture documentation
dump/
  sports2000.df          - Database schema definition
```

## Prerequisites

- OpenEdge 12.8+
- Sports2000 sample database

## Getting Started

1. Clone this repository
2. Create the Sports2000 database: `ant db`
3. Open in Progress Developer Studio or compatible IDE
4. Run `CustomerWin.w` or `ItemWin.w`
