# Read the Raspberry Pi temperature

## Temperature from the terminal

Here, we are using the Pi as if it was a temomether. To do so, let's track its temperature. Open a terminal and type:

```bash
vcgencmd measure_temp
```

Submit an image with the 

## Do the same in python

Now, create a Python file with the following content :

```python
import subprocess

def read_temp():
    output = subprocess.check_output(["vcgencmd", "measure_temp"])
    temp_str = output.decode()  # e.g., "temp=47.8'C"
    temp_value = float(temp_str.replace("temp=", "").replace("'C", ""))
    return temp_value

if __name__ == "__main__":
    print("Temperature:", read_temp())

<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/37944562-b9b7-41aa-b66e-4cfae66fea38" />


```

and run it in a terminal:

```bash
python3 read_temp.py
```

