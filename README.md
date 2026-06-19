# Lab 6 - HashMap Implementation

## Description

This lab focuses on creating and using a custom HashMap in Java. The program uses a `MyMap` interface and a `MyHashMap` class to store course numbers and their credit hours as key-value pairs. The course number acts as the key, and the number of credit hours acts as the value.

The lab also practices common HashMap operations such as adding entries, checking if a key exists, printing the map contents, removing entries, and printing only the values.

## Files Included

* `Main.java`
* `MyMap.java`
* `MyHashMap.java`
* `instructions.md`

## Program Features

This program completes the following tasks:

* Creates a map called `creditHours`
* Adds course numbers and credit hours using `put()`
* Checks whether certain course keys exist in the map
* Prints all key-value pairs in the map
* Removes selected courses from the map
* Prints only the remaining credit-hour values

## Course Data Used

The following course numbers and credit hours were added to the map:

```java
creditHours.put("IT-1025", 3);
creditHours.put("IT-1050", 3);
creditHours.put("IT-1150", 3);
creditHours.put("IT-2310", 3);
creditHours.put("IT-2320", 4);
creditHours.put("IT-2351", 4);
creditHours.put("IT-2650", 4);
creditHours.put("IT-2660", 4);
creditHours.put("IT-2030", 4);
```

## Key Checks

The program checks whether the map contains these keys:

```java
creditHours.containsKey("IT-1025");
creditHours.containsKey("IT-2110");
```

`IT-1025` should return `true` because it was added to the map.
`IT-2110` should return `false` because it was not added to the map.

## Removed Entries

The following entries were removed from the map:

```java
creditHours.remove("IT-2030");
creditHours.remove("IT-1150");
```

## Expected Output

The exact order of the HashMap output may be different because HashMaps do not always print items in insertion order. However, the output should show that `IT-1025` exists, `IT-2110` does not exist, all course entries are printed, and then only the remaining credit-hour values are printed after removing two courses.

Example output:

```text
Does the map contain IT-1025? true
Does the map contain IT-2110? false

All courses and credit hours:
[[IT-1025, 3][IT-1050, 3][IT-1150, 3][IT-2310, 3][IT-2320, 4][IT-2351, 4][IT-2650, 4][IT-2660, 4][IT-2030, 4]]

Credit hour values after removing IT-2030 and IT-1150:
[3, 4]
```

## What I Learned

In this lab, I learned more about how HashMaps store data using key-value pairs. I practiced using keys to quickly find values, checking whether a key exists, removing entries, and printing map contents. I also learned that HashMaps are useful because they allow fast lookup, insertion, and removal of data.
