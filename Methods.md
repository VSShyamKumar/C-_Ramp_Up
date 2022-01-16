What is Lasagne : https://en.wikipedia.org/wiki/Lasagne

![Pic Lasagne](https://upload.wikimedia.org/wikipedia/commons/thumb/b/ba/Lasagne_-_stonesoup.jpg/878px-Lasagne_-_stonesoup.jpg)


Question : 


Sol 1 simple and straight forward.
```c#
class Lasagna
{
    public int ExpectedMinutesInOven()
    {
        return 40;
    }

    public int RemainingMinutesInOven(int actualMinutesInOven)
    {
        return ExpectedMinutesInOven() - actualMinutesInOven;
    }

    public int PreparationTimeInMinutes(int numberOfLayers)
    {
        return numberOfLayers * 2;
    }

    public int ElapsedTimeInMinutes(int numberOfLayers, int actualMinutesInOven)
    {
        return PreparationTimeInMinutes(numberOfLayers) + actualMinutesInOven;
    }
}
```

Solution 2 kind of pro level (using Lambda Expressions)
```c#
class Lasagna
{
    public int ExpectedMinutesInOven() => 40;
    public int RemainingMinutesInOven(int minutesInOven) => ExpectedMinutesInOven() - minutesInOven;
    public int PreparationTimeInMinutes(int numberOfLayers) => numberOfLayers * 2;
    public int ElapsedTimeInMinutes(int numberOfLayers, int minutesInOven) => PreparationTimeInMinutes(numberOfLayers) + minutesInOven;
}
```

