layout: page
title: "Moto Rates - Rwanda"
permalink: /rates/rw/
apiVersion: schemas.schemahero.io/v1alpha4
kind: Table
metadata:
  name: session
spec:
  database: my-database
  name: session
  schema:
    postgres:
      primaryKey:
      - id
      columns:
      - name: id
        type: text
        constraints:
          notNull: true
      - name: user_id
        type: text
        constraints:
          notNull: true
      - name: expire_at
        type: timestamp without time zone
        constraints:
          notNull: true
