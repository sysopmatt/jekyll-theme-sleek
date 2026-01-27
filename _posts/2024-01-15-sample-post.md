---
layout: post
title: "Sample Post with Code Examples"
date: 2024-01-15
tags: [sample, code, tutorial]
---

This is a sample blog post demonstrating code syntax highlighting.

## JavaScript Example

```javascript
const greet = (name) => {
  return `Hello, ${name}!`;
};

// Using the function
const message = greet('World');
console.log(message);
```

## Python Example

```python
class DataProcessor:
    def __init__(self, data):
        self.data = data

    def process(self):
        """Process the data and return results."""
        results = []
        for item in self.data:
            results.append(item * 2)
        return results

# Usage
processor = DataProcessor([1, 2, 3, 4, 5])
print(processor.process())  # [2, 4, 6, 8, 10]
```

## SQL Example

```sql
SELECT
    users.name,
    COUNT(orders.id) AS order_count
FROM users
LEFT JOIN orders ON users.id = orders.user_id
WHERE users.created_at >= '2024-01-01'
GROUP BY users.id
HAVING COUNT(orders.id) > 5
ORDER BY order_count DESC;
```

## Bash Example

```bash
#!/bin/bash

# Deploy script
echo "Starting deployment..."

git pull origin main
npm install
npm run build

echo "Deployment complete!"
```

## YAML Example

```yaml
name: Deploy Site
on:
  push:
    branches: [main]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Build
        run: npm run build
```

That's all for the code examples!
