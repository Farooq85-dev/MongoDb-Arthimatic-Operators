# MongoDb-Arthimatic-Operators

### What are Arthimatic operators in MongoDB?

#### In MongoDB, arithmetic operators are used to perform mathematical operations on data within aggregation pipelines.

### 1) `add`

#### Adds numbers or concatenates strings.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $add: ["$price", 100]
      }
    }
  }
])
```

### 2) `substract`

#### Subtracts one number from another.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $subtract: ["$price", 2]
      }
    }
  }
])
```

### 3) `substract`

#### Subtracts one number from another.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $subtract: ["$price", 2]
      }
    }
  }
])
```

### 4) `multiply`

#### Multiplies numbers together.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $multiply: ["$price", 2]
      }
    }
  }
])
```

### 5) `mod`

#### Returns the remainder of a division operation.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $mod: ["$price", 2]
      }
    }
  }
])
```

### 6) `abs`

#### Returns the absolute value of a number (ignores negative signs).

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $abs: ["$price"]
      }
    }
  }
])
```

### 7) `ceil`

#### Rounds a number up to the nearest integer.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $ceil: ["$price"]
      }
    }
  }
])
```

### 8) `floor`

#### Rounds a number up to the nearest integer.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $floor:["$price"]
      }
    }
  }
])
```

### 9) `round`

#### Rounds a number to a specified decimal place.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $round:["$price"]
      }
    }
  }
])
```

### 10) `sqrt`

#### Returns the square root of a number.

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $sqrt:["$price"]
      }
    }
  }
])
```

### 11) `pow`

#### Raises a number to a specified exponent (base^exponent).

```
db.collection.aggregate([
  {
    $project: {
      newPrice: {
        $pow:[ "$base", 2 ] // Square the value of base
      }
    }
  }
])
```
