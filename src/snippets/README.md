# Visual Studio Snippets

The files in this directory are Visual Studio "intellisense snippets."

To use these snippets in your copy of Visual Studio, copy them into the `VC#\Snippets\1033\Visual C#` folder under your Visual Studio directory, or add it using the Code Snippets Manager (**Ctrl+K, Ctrl+B**).


## `mvlprop` (MVVM Light Property)

For use with an `ObservaleObject`, this code snippet creates a Property (including a corresponding private member) including a setter which calls the `Set` method.

### Compatibility
`C#`

### Usage
`mvlprop <TAB> <TAB>`

### Example
```c#
private int mProperty;

public int Property
{
  get { return mProperty; }
  set { Set<int>(() => this.mProperty, ref mProperty, value); }
}
```


## `mvlpropc` (MVVM Light Collection Property)

This code snippet creates an `ObservableCollection<T>` Property (including a corresponding private member) with a public getter and no setter.

### Compatibility
`C#`

### Usage
`mvlpropc <TAB> <TAB>`

### Example
```c#
private ObservableCollection<int> mProperty = new ObservableCollection<int>();

public ObservableCollection<int> Property
{
  get { return mProperty; }
}
```
