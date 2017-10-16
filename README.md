### SortArrays

I have a List<> containing data. How can I sort it to ascending and descending?
================================================================

Sorting List ascending and descending android java
================================================================

### Prerequisites
What things you need to install the software and how to install them

![attachment](https://user-images.githubusercontent.com/16405013/31633829-e08b2f34-b2c1-11e7-8ba8-62b6608eb0ae.png)

================================================================






Colons can be used to align columns.

| different        | descending           | ascending  |
| ------------- |:-------------:| -----:|
| ![attachment](https://user-images.githubusercontent.com/16405013/31634540-393872e8-b2c4-11e7-8dc3-059154f8f77d.png)     |![attachment](https://user-images.githubusercontent.com/16405013/31634595-6161870a-b2c4-11e7-8dd7-9d61afd9f27f.png) | ![attachment](https://user-images.githubusercontent.com/16405013/31634612-6d969e84-b2c4-11e7-8118-fc739832ffe1.png) |




Usage
-----

Basic form:
Let your class implement the Comparable interface, this lets Java handle most of the heavy lifting.

```ruby
public class Data implements Comparable<Data>{
    @Override
    public int compareTo(Data another) {
        return this.title.compareTo(another.title);
        // can also compareToIgnoreCase if not case sensitive
    }
}
```

Then simply call Collections.sort(data);
This will sort your data based on the compareTo function in your Data class.
