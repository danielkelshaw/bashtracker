## **bashtracker**
Simple bash script for tracking simple values from the command line.

### **Setup:**

Clone the repository and change directory:

```bash
git clone https://github.com/danielkelshaw/bashtracker
cd bashtracker
```

Add the `src` directory to your path:

```bash
echo "export PATH=\"\$PATH:$(pwd)/src\"" >> ~/.zshrc
```

### **Track a Quantity:**

```bash
track <name> <value>
```

This will create a file at: `/path/to/repo/notes/<name>.csv` with the current DateTime and value.

### **Sum a Quantity:**

```bash
track --sum <name> <-n[mdY]>
```

This will provide a sum of the values in the last `<-n[mdY]>`

### **Count a Quantity:**

```bash
track --count <name> <-n[mdY]>
```

This will count the number of occurences in the last `<-n[mdY]>`

### **Show a Quantity:**

```bash
track --show <name>
```

This will `cat` out the relevant file - displaying the contents.

### **Clear Tracking:**

```bash
track --clear <name>
```

This will delete the file at: `/notes/<name>.csv`.

###### Made by Daniel Kelshaw
