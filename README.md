# HashMap in Java

This is a simple demonstration of using the `HashMap` class in Java to store key-value pairs and perform basic operations like accessing keys, values, entries, and removing elements.

## What is a HashMap?

A `HashMap` is a collection class that implements the `Map` interface. It stores key-value pairs, where each key is associated with a value. The `HashMap` class allows for fast lookups, additions, and removals based on keys, making it an efficient data structure for managing collections of key-value mappings.

### Key Features of HashMap:
- **Key-Value Pair**: A `HashMap` stores elements in the form of key-value pairs. Each key is unique, but different keys can have the same value.
- **Efficient Operations**: It provides constant-time performance (O(1)) for basic operations like `get`, `put`, and `remove`, assuming the hash function disperses the elements properly.
- **Unordered**: `HashMap` does not maintain any specific order of its entries (keys and values). The order of entries may change when new entries are added or removed.

## Code Explanation

In the provided Java code, we perform several operations on a `HashMap` object named `numbers`:

1. **Creating the HashMap**:
   - A `HashMap` is initialized where the key type is `String` and the value type is `Integer`.

2. **Adding Entries**:
   - The `put()` method is used to add key-value pairs to the `HashMap`. We add `"One"` as the key with value `1`, and `"Two"` as the key with value `2`.

3. **Printing the Map**:
   - We print the entire `HashMap`, which displays the key-value pairs stored in the map.

4. **Accessing Keys**:
   - The `keySet()` method returns a `Set` of all the keys in the map, which are printed.

5. **Accessing Values**:
   - The `values()` method returns a collection of all the values in the map, which are printed.

6. **Accessing Entries**:
   - The `entrySet()` method returns a `Set` of key-value pairs (entries), which are printed.

7. **Removing an Entry**:
   - The `remove()` method is used to remove an entry by specifying the key (`"Two"`). The method returns the value associated with the removed key, which is printed.

### Code
```Java
import java.util.Map;
import java.util.HashMap;

public class HashMapDemo {

    public static void main(String[] args) {
        Map<String, Integer> numbers = new HashMap<>();
        numbers.put("One", 1);
        numbers.put("Two", 2);
        System.out.println("Map:" + numbers);
        System.out.println("Keys:" + numbers.keySet());
        System.out.println("Values:" + numbers.values());
        System.out.println("Entries:" + numbers.entrySet());
        int value = numbers.remove("Two");
        System.out.println("Removed Value: " + value);
    }
}
```
### Output
```
Map:{One=1, Two=2}
Keys:[One, Two]
Values:[1, 2]
Entries:[One=1, Two=2]
Removed Value: 2
```

As shown in the output:
- The `Map:{One=1, Two=2}` prints the entire `HashMap` containing the key-value pairs.
- The `Keys:[One, Two]` prints all the keys in the map.
- The `Values:[1, 2]` prints all the values in the map.
- The `Entries:[One=1, Two=2]` prints all key-value pairs (entries) in the map.
- The `Removed Value: 2` shows the value associated with the key `"Two"`, which was removed from the map.

## Key Methods in HashMap:

- **put(K key, V value)**: Adds the specified key-value pair to the map. If the key already exists, the value is updated.
- **get(Object key)**: Retrieves the value associated with the specified key.
- **keySet()**: Returns a `Set` of all the keys in the map.
- **values()**: Returns a collection of all the values in the map.
- **entrySet()**: Returns a `Set` of all the key-value pairs (entries) in the map.
- **remove(Object key)**: Removes the key-value pair associated with the specified key.
- **containsKey(Object key)**: Checks if the map contains the specified key.
- **containsValue(Object value)**: Checks if the map contains the specified value.
- **size()**: Returns the number of key-value pairs in the map.
- **clear()**: Removes all key-value pairs from the map.

## Conclusion

The `HashMap` class is a powerful and efficient data structure for working with key-value pairs in Java. It allows for quick lookups, additions, and removals, making it ideal for scenarios where you need to associate keys with values and perform fast searches.

Feel free to experiment with different operations and explore more features of the `HashMap` class in Java!


