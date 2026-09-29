# RDB HW-02: Database Normalization

## Task Condition
Normalize the given database schema to **1NF, 2NF, and 3NF** based on the provided entity-relationship diagram (`erDiagram.png`).
The initial schema is represented in `initial_table.jpg`.

### Requirements:
1. **1NF (First Normal Form)**:
   - Eliminate repeating groups.
   - Ensure atomic values in each cell.
   - Result: `p1_1NF.png`

2. **2NF (Second Normal Form)**:
   - Meet 1NF requirements.
   - Remove partial dependencies (all non-key attributes must depend on the entire primary key).
   - Result: `p2_2NF.png`

3. **3NF (Third Normal Form)**:
   - Meet 2NF requirements.
   - Remove transitive dependencies (non-key attributes must not depend on other non-key attributes).
   - Result: `p3_3NF.png`

### Schema Details:
The database includes the following entities (screenshots in `shema_screenshots/`):
- `client`
- `order`
- `order_items`
- `products`

## Conclusion
The database was successfully normalized to **3NF** by:
1. Decomposing the initial table into atomic structures (1NF).
2. Eliminating partial dependencies by splitting composite keys (2NF).
3. Removing transitive dependencies by isolating derived attributes (3NF).

Each normalization step is documented in the respective `.png` files.