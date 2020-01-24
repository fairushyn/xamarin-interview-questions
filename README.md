# Xamarin Interview Questions and Answers

C# is one of the top 5 languages that people use around the world and the app-building over the Xamarin platform is on rise. Xamarin is a prominent choice among developers and the reason behind it is — “ Seamless Functionality”. Launched in 2011, Xamarin offers code re-usability and sharing codes with other platforms while giving access to native API’s.

> You could also find all the answers here 👉 https://www.fullstack.cafe/Xamarin.

<p align="center">
  <a href="https://www.fullstack.cafe">
  <img src="https://user-images.githubusercontent.com/13550565/73042889-e7533900-3e9d-11ea-94f2-b4a9e87cc018.png">
  </a>
</p>

## Q1: What is Xamarin? ⭐

**Answer:**

**Xamarin** is a Cross Platform Mobile Development technology by Microsoft where we can develop the native app using the same code base across all platforms (iOS, Android, UWP) using the C# language. Xamarin uses two approaches for the app development:
* Xamarin.Forms and 
* Xamarin Native. 

Xamarin.Forms uses MVVM & XAML while Xamarin Native uses native UI technology and MVC or MVVMCross Architecture.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q2: What is is the difference between ListView & TableView? ⭐⭐

**Answer:**

The ListView and TableView controls are so similar, you can think of them as a single control. The major difference between the two is the manner in which they lay out their items, and it’s easy to change the layout so each control emulates the other.

* The ListView control displays its data stacked vertically, much like a standard listbox. Use this control to display an ordered list of data, especially long lists that require scrolling like a list of email messages, a list of contacts, or search results.

* The TableView control displays its data stacked horizontally in rows (although you can alter this behavior and have it displayed in columns first, as well). You use this control when you need more space for rich visualization of each item to be displayed.

One of the big differences is ListView provides you a ItemsSource and a Itemtemplate and TableView does not. So items must be added as children manually.

🔗 **Source:** [greenstechnologys.com](http://www.greenstechnologys.com/xamarin-interview-questions.html)


## Q3: How to display static HTML string in Xamarin.Forms? ⭐⭐

**Answer:**

We can use WebView control to display `static` HTML `string`. `WebView` can be used to display Websites, HTML string, Documents, Local Files depending on the platform support.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q4: How to store simple Key-Value data? ⭐⭐

**Answer:**

Xamarin.Forms's `Application` class exposes the `Application.Current.Properties` `Dictionary` which is used to store the simple Key-Value pair data. The `Properties` dictionary uses a `string` key and stores an object value.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q5: What is the difference between Margin and Padding properties? ⭐⭐

**Answer:**

* `Margin` property represents the distance between the element and its adjacent elements and is used to control the element's rendering position, and the rendering position of its neighbors. Margin can be specified on `Layout` and `View` classes.

* `Padding` property represents the distance between an `Element` and the child elements of it and thus it is used to separate the control from its own content. `Padding` values can be specified on `Layout` classes.

Suppose, two adjacent elements have a margin of value 20 pixels assigned, what will be the distance between these two elements? Why?

The distance between two elements will be 40 pixels in this case, because, `Margin` property values are `Additive`. In addition to this, if `Margin` and `Padding` both are applied, then the distance between element and its content will be `Margin + Padding`.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q6: Name few widely used Layout Controls ⭐⭐

**Answer:**

*   `Frame`: It contains a single element as a child having a default padding of 20.
*   `Grid`: It is used when UI components are to be arranged into Rows & Columns.
*   `StackLayout`: It is used when UI components are to be arranged either horizontally or vertically.
*   `ScrollView`: It enables the scrolling for a child element if required. It has one child only.

There are other Layout Controls too like `AbsoluteLayout`, `RelativeLayout`, `ContentView`, `ContentPresenter`, etc.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q7: How will you navigate from one page to another? ⭐⭐

**Answer:**

On some button click event of First Page, we can call the following method, which will navigate to the second page:

```csharp
await Navigation.PushAsync (new MySecondPageXaml (), true);
```

We have to use the "`Navigation`" property which is available under `ContentPage` class (XAML Page's code behind). So this navigation can be written in the Page's code behind file.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q8: Explain Lifecycle methods of Xamarin.Forms app ⭐⭐

**Answer:**

Lifecycle methods are set of methods which get executed when application enters into a specific state. Following are such methods:

*   `OnStart`: Executes when application starts from the beginning
*   `OnSleep`: Executes each time when application goes into the background
*   `OnResume`: Executes when application comes into the foreground from the Sleeping state

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q9: What is App.cs class? ⭐⭐

**Answer:**

_App.cs_ is the main class of the app which offers features like:

*   **MainPage**: It helps to set the initial page for the app.
*   **Properties Dictionary**: It helps us store simple values across lifecycle states.
*   **Static Current Property**: It gives the instance of the current application object.

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q10: What is the basic architecture of Xamarin.Forms project? ⭐⭐

**Answer:**

Xamarin.Forms can consists of four (this varies based on requirements) projects under one solution.

*   .NET Standard, PCL or Shared Project
*   iOS Project
*   Android Project
*   UWP Project

Here, .NET Standard, PCL or Shared Project contains all UI & Business logic inside it.

iOS, Android, UWP contains platform specific code containing Renderers or Dependency Services Implementations.


🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q11: Which Languages are supported for Xamarin development? ⭐⭐

**Answer:**

C# & F#

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q12: What is Xamarin.Forms and what are the benefits of using it? ⭐⭐

**Answer:**

**Xamarin.Forms** is a Cross-Platform Toolkit which helps share Business Logic as well as UI using XAML across all supported platforms.

It uses MVVM pattern along with Binding into the XAML UI to accomplish this. It produces pure native controls for each individual platforms. Using Xamarin.Forms, we can share the whole business logic as well as UI among all supporting platforms like iOS, Android and UWP. It also provides a way for platform specific customization of any native controls using Renderers. Thus, we can almost share about 80-90% of code across platforms. We can say Xamarin is the King of Cross Platforms.


🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q13: What is the difference between Xamarin.Forms & Xamarin Native? ⭐⭐

**Answer:**

Xamarin.Forms is used when:

*   Less platform-specific code is required
*   Code sharing is more important than custom UI
*   UI is not complex

Xamarin Native is used when:

*   Lot of platform specific code is required
*   Custom UI is more important then code sharing
*   Many platform-specific APIs are used

🔗 **Source:** [codeproject.com](https://www.codeproject.com/Articles/1231821/Xamarin-Questions-Answers)


## Q14: What are the various flavors of Xamarin Applications that can be made? ⭐⭐

**Answer:**

Xamarin allows two different ways of creating applications, based on the amount of code reusability and customization:

* The first approach is the **Traditional Native Approach** wherein platform-specific apps using Xamarin.iOSiOS and Xamarin.Android can be made. This way of creating apps is generally used when there is a lot of customization specific to the platform is required as it allows direct access to platform-specific APIs. Xamarin.iOS is used for iOS applications and Xamarin.Android is used to create Android applications.

* The second approach is creating apps through **Xamarin.Forms approach**. Xamarin.Forms are used when there is a possibility of reuse of a lot of platform-independent code and the focus is less on custom UI. The platform-independent code is separated and kept in Shared Project or PCL or .NET Standard Library and Platform Specific projects consume this common code by including it.

🔗 **Source:** [knowledgehut.com](https://www.knowledgehut.com/interview-questions/xamarin)


## Q15: What are Pages in Xamarin.Forms? ⭐⭐

**Answer:**

**Pages** are Xamarin Forms generic representation of Cross Mobil Application Screens. A Page occupies most or all of a screen and contains a single child.

On IOS, the Page is mapped to ViewController, on Android, it is mapped to somewhat like Activity and on Universal Windows Platform, it is mapped to  Page. Pages can be of several types, viz. Master /Detail Page, navigational Page, Carousel Page, Tabbed Page, Template Page, etc.

🔗 **Source:** [knowledgehut.com](https://www.knowledgehut.com/interview-questions/xamarin)


## Q16: What is TestFlight? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q17: What is the difference between Xaml & Axml in Xamarin Technology? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q18: What is the difference between Xamarin.Forms and Xamarin Native? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q19: How to perform Binding in Code Behind? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q20: What is View-to-View Binding? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q21: What are Triggers? How many types of Triggers are available? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q22: What is the purpose of INotifyPropertyChanged? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q23: What is difference between ControlTemplate & DataTemplate? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q24: What is Custom Renderers and what is its purpose? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q25: What is Behaviors and give some examples where we should use Behaviors? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q26: What is the special meaning with "AndExpand" Suffix with each LayoutOptions? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q27: What is ViewCell and How many types of built-in Cells are available? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q28: What is the purpose of InitializeComponent() method in Page? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q29: When would you use the NavigationPage as a MainPage? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q30: What is ResourceDictionary? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q31: What is XAML Markup Extensions? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q32: What is the purpose of XAML Compiler (XAMLC)? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q33: What is the difference between PCL & Shared Project? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q34: How many ways can we share the code? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q35: How many types of Pages are available in Xamarin.Forms? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q36: How to do Xamarin.Android applications work? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q37: How To Share Code Between Cross-Platform Applications on Xamarin? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q38: How To Share Code Between Cross-Platform Applications on Xamarin? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q39: Explain .NET Standard Libraries For Sharing Code on Xamarin? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q40: Explain how to use shared projects in Xamarin? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q41: What is Dependency Service and how it functions on Xamarin.Forms? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q42: What are Custom renderers in Xamarin.Forms? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q43: What are Effects and when should they be used? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q44: What is Fresh MVVM? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q45: What are the advantages and disadvantages of using XAML in Xamarin.Forms? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q46: What is info.plist in Xamarin.iOS ? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q47: How to call a specific method for some specific Platform only? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q48: What is MessagingCenter? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q49: Is there any benefit in binding a ViewModel in backend .cs file? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q50: How many ways you can Bind a ViewModel with XAML? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q51: How many ways we can Bind data? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q52: How do we provide Platform specific styling or values in XAML? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q53: How to design separate layouts or functionality between Phone & Tablets? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q54: What are the disadvantages of Xamarin for Android development? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q55: What is DependencyService? Describe steps for the implementation. ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q56: What is Effects and When should we use it over Custom Renderers? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q57: Which best practices to follow while designing the XAML Page? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q58: How to render different types of ViewCell in the same ListView during runtime? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q59: Why do we need to create a Custom ViewCell? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q60: How many types of different XAML Markup Extensions do you know? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q61: What are some features of Fresh MVVM? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q62: What is MVVM Cross? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q63: What is MVVM Light ? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q64: Name some types of Behaviors in Xamarin? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q65: What is the difference between Entry and Editor in Xamarin.Forms? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q66: Name some types of keys defined in info.plist files ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q67: How to make iOS native libraries accessible in Xamarin apps? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q68: What are Services in Xamarin.Android? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q69: What the Xamarin platform consists of? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q70: How does compilation work for Xamarin? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q71: What is Xamarin.Essentials? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q72: What is the disadvantage of Xamarin to using for example Objective-C or Java for iOS and Android separately? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q73: So, what is the difference between MessagingCenter and Events? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q74: Can we really declare Parametrized ViewModel instance as BindingContext in XAML? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q75: How to increase the ListView performance? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q76: What are provisioning profiles on Xamarin.iOS? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q77: Explain what is linking process on Xamarin ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q78: Name some limitation of Xamarin.iOS ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q79: What are Android Callable Wrappers (ACWs)? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q80: Explain what happens when the Xamarin.Android application compiles? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q81: Why AOT is used for Xamarin.iOS? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q82: What is Selector in Xamarin.iOS? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**


## Q83: What is Registrar in Xamarin.iOS? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Xamarin)**



