![Many to Many Schema Design Examples](http://i.imgur.com/N64Hdlp.png)


Many to Many Design

- Recognizing design patterns is a useful "tool" in building relational databases and modeling an enterprise.
- Using english phrases can help determine which design pattern to implement.
  Examples of many to many:

  "Each movie contains one or more actors"
  "Each actor is contained by one or more movies"

  "Each order contains one or more products"
  "Each product is contained in zero or more orders"
  (Zero because we might not have sold any of this product yet)

  "Each chinese character contains one or more radicals"
  "Each radical is contained in one or more chinese characters"

  "Each artistic movement contains one or more artists"
  "Each artist is contained in one or more artistic movements"

- We can't represent a many-to-many association directly in a relation scheme, because towo tables can't be children of each other.
  (There is no place for foreign keys)

- Every many-to-many requires a junction table.
  Junction tables can also be called a join or linking table.
  This junction table holds the foreign keys that connect each side of the association.

- If attributes result from a many-to-many association, we can show them in an association class.
  Often this association class (list of shared attributes) is added into the junction table.
  *Recall the class - grade - student example from our core challenges this week
  *See the orders_products table for further reference


