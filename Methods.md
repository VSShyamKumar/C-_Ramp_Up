What is Lasagne : https://en.wikipedia.org/wiki/Lasagne

![Pic Lasagne](https://en.wikipedia.org/wiki/File:Lasagne_-_stonesoup.jpg)


```c#
class Lasagna
{
    public int ExpectedMinutesInOven() => 40;
    public int RemainingMinutesInOven(int minutesInOven) => ExpectedMinutesInOven() - minutesInOven;
    public int PreparationTimeInMinutes(int numberOfLayers) => numberOfLayers * 2;
    public int ElapsedTimeInMinutes(int numberOfLayers, int minutesInOven) => PreparationTimeInMinutes(numberOfLayers) + minutesInOven;
}
```
