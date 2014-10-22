Some scripts to access the data streamed by the **Neurosky Mindwave Mobile** Headset over Bluetooth on Linux.

Requirements:
* [PyBluez](http://code.google.com/p/pybluez/), see their [documentation](http://code.google.com/p/pybluez/wiki/Documentation) for installation instructions :)
For Ubuntu, installation might work like this:
```
sudo apt-get install libbluetooth-dev
pip install pybluez
```


If you want to install the library as a module, do:
```
python setup.py install
```
from the root folder of the repository.

Afterwards, you can use it within python like this:

```python
from mindwavemobile.MindwaveDataPointReader import MindwaveDataPointReader
mindwaveDataPointReader = MindwaveDataPointReader()
# connect to the mindwave mobile headset...
mindwaveDataPointReader.start()
# read one data point, data point types are specified in  MindwaveDataPoints.py'
dataPoint = mindwaveDataPointReader.readNextDataPoint()
``` 
You're probably wondering, "pcbmaster, why should I use your fork?"
The answer is simple
Don't


I'm not fucking kidding don't use this

It's so broken
