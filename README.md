# Books

2018.2.1  

windows核心编程

windows内核安全与驱动开发


MSDN开发人员代码示例

[https://code.msdn.microsoft.com](https://code.msdn.microsoft.com)

[https://developer.xamarin.com/samples/xamarin-forms/all/](https://developer.xamarin.com/samples/xamarin-forms/all/)

<br/><br/>

wpf  -   prism和mvvmlight中DelegateCommand、RelayCommand对比

在command source 是否启动的处理上的差异：
RelayCommand使用RoutedCommand相同的逻辑(注册过多，会影响程序性能)：
```
  public event EventHandler CanExecuteChanged
	{
	  add
		{
			CommandManager.RequerySuggested += value;
		}
		remove
		{
			CommandManager.RequerySuggested -= value;
		}
 }
```

DelegateCommand使用主动通知进行优化：
```
    public void RaiseCanExecuteChanged()
      {
          OnCanExecuteChanged();
      }
```

<br/><br/>
[流畅设计 Fluent Design System 中的光照效果 RevealBrush，WPF 也能模拟实现啦！](https://walterlv.com/post/fluent-design-reveal-brush-in-wpf.html)
