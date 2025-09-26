# 01: Syntax

This guide provides an overview of YAML's core syntax, which is used to represent data in a human-readable format.

---

## Comments

The hash symbol (`#`) marks the beginning of a comment. Everything from the hash to the end of the line is ignored by the parser.

```yaml
# This is a comment.
```

---

## Key-Value Pairs

A **key-value pair** associates a name (the key) with a piece of data (the value).

- **Keys**: A key is followed by a colon and a space (`: `), and then its value.

- **Values**: Values can be simple data types like strings, numbers, or booleans.

```yaml
# A key named 'name' with a string value
name: John Doe

# A key named 'age' with a number value
age: 42

# A key named 'is_employed' with a boolean value
is_employed: true
```

---

## Indentation and Structure

YAML uses indentation to define the structure of the data. Nesting is achieved by indenting a block of key-value pairs under a parent key. The standard convention is to use two spaces for each level of indentation.

```yaml
# 'address' is a parent key.
# 'street' and 'city' are nested inside 'address'.
address:
  street: 123 Main St
  city: Anytown
```

---

## Lists (Sequences)

A list is a collection of items where the order matters. Each item in a list begins with a dash and a space (`- `).

```yaml
# A list of skills
skills:
  - Python
  - JavaScript
  - YAML

# A list can also contain more complex objects, like dictionaries
projects:
  - name: Project Alpha
    status: In Progress
  - name: Project Beta
    status: Complete
```

---

## Dictionaries (Mappings)

A dictionary is a collection of key-value pairs.

```yaml
# The 'user' key holds a dictionary.
# This dictionary contains three key-value pairs: id, email, and role.
user:
  id: 101
  email: user@example.com
  role: admin
```
