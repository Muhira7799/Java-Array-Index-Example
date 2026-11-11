# Java Array Index Example

A small Java program that shows how to read a single element from an array using its index.

## What It Demonstrates

```java
int[] marks = {10, 12, 13, 15, 17, 19, 20};
System.out.println("Element at index 4: " + marks[4]);
```

Array indexes start at `0`, so index `4` is the fifth element.

| Index | 0 | 1 | 2 | 3 | 4 | 5 | 6 |
|-------|---|---|---|---|---|---|---|
| Value | 10 | 12 | 13 | 15 | **17** | 19 | 20 |

## Output

```
Element at index 4: 17
```

## Note on the Name

Despite the class name `Average`, the program does not calculate an average. It only prints one element. To calculate the average of the array, add the values and divide by the length:

```java
int sum = 0;
for (int m : marks) {
    sum += m;
}
double average = (double) sum / marks.length;
System.out.println("Average: " + average);
```

For these marks, the average is about `15.14`.

## Common Error

Using an index that is too large, such as `marks[7]`, throws an `ArrayIndexOutOfBoundsException`, because the valid indexes here are `0` to `6`.

## Requirements

- Java Development Kit (JDK) 8 or higher

## Getting Started

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
javac Average.java
java Average
```

## Project Structure

```
.
├── Average.java
└── README.md
```

## Next Steps

- Add the average calculation shown above
- Print the first and last elements
- Use `marks.length - 1` to always get the last element
