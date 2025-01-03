# Bubble Sort

Bubble sort is an easy way to sort a list. It goes through the list over and over. Each time, it looks at two items next to each other. If they are in the wrong order, it swaps them. It keeps doing this until everything is sorted. It's called bubble sort because smaller items bubble up to the top of the list.

<table>
    <tbody>
        <tr>
            <td className="bg-amber-600">5</td>
            <td className="bg-amber-600">3</td>
            <td>13</td>
            <td>2</td>
            <td>11</td>
            <td>4</td>
            <td>7</td>
        </tr>
    </tbody>
</table>

5 and 3 are in the wrong order, so they are swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td className="bg-amber-600">5</td>
            <td className="bg-amber-600">13</td>
            <td>2</td>
            <td>11</td>
            <td>4</td>
            <td>7</td>
        </tr>
    </tbody>
</table>

5 and 13 are in the right order, so they are not swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td>5</td>
            <td className="bg-amber-600">13</td>
            <td className="bg-amber-600">2</td>
            <td>11</td>
            <td>4</td>
            <td>7</td>
        </tr>
    </tbody>
</table>

13 and 2 are in the wrong order, so they are swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td>5</td>
            <td>2</td>
            <td className="bg-amber-600">13</td>
            <td className="bg-amber-600">11</td>
            <td>4</td>
            <td>7</td>
        </tr>
    </tbody>
</table>

13 and 11 are in the wrong order, so they are swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td>5</td>
            <td>2</td>
            <td>11</td>
            <td className="bg-amber-600">13</td>
            <td className="bg-amber-600">4</td>
            <td>7</td>
        </tr>
    </tbody>
</table>

13 and 4 are in the wrong order, so they are swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td>5</td>
            <td>2</td>
            <td>11</td>
            <td>4</td>
            <td className="bg-amber-600">13</td>
            <td className="bg-amber-600">7</td>
        </tr>
    </tbody>
</table>

13 and 7 are in the wrong order, so they are swapped.

<table>
    <tbody>
        <tr>
            <td>3</td>
            <td>5</td>
            <td>2</td>
            <td>11</td>
            <td>4</td>
            <td>7</td>
            <td className="bg-green-600">13</td>
        </tr>
    </tbody>
</table>

The last element is now in the right place. The process is repeated until the remaining elements are sorted.

## Pseudo Code

```plaintext
function bubbleSort(arr)
    n = arr.length
    for i = 0 to n - 1
        for j = 0 to n - i - 1
            if arr[j] > arr[j + 1]
                swap(arr[j], arr[j + 1])
```

## Explanation

1. The outer loop goes through the list from the beginning to the end.
2. The inner loop goes through the list from the beginning to the end minus the current position of the outer loop. This is because after every iteration of the outer loop, the largest element is placed at the end of the list.
3. If the current element is greater than the next element, they are swapped.
4. The process is repeated until the list is sorted.

## Complexity Analysis

-   Running time complexity: $O(n^2)$\
-   Space complexity: $O(1)$
-   Best-case time complexity: $O(n)$
    > The best-case time complexity is O(n) when the list is already sorted.
-   Average-case time complexity: $O(n^2)$
-   Worst-case time complexity: $O(n^2)$

### test h3
#### test h4