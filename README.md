# Xamarin Navigation Drawer (SfNavigationDrawer) 

This section explains you the steps required to create a navigation DrawerPanel with content area and data filled drawer and it covers only the minimal features that you need to know to get started with the NavigationDrawer.

For know more details about NavigationDrawer: https://www.syncfusion.com/xamarin-ui-controls/xamarin-navigation-drawer

NavigationDrawer user guide documentation: https://help.syncfusion.com/xamarin/navigation-drawer/getting-started

## Assembly deployment
After installing Essential Studio for Xamarin, you can find all the required assemblies in the installation folders, {Syncfusion Essential Studio Installed location} \Essential Studio\{Version #}\Xamarin\lib.

## Adding SfNavigationDrawer reference
You can add SfNavigationDrawer reference using one of the following methods:

## Method 1: Adding SfNavigationDrawer reference from nuget.org

Syncfusion Xamarin components are available in nuget.org. To add SfNavigationDrawer to your project, open the NuGet package manager in Visual Studio, search for Syncfusion.Xamarin.SfNavigationDrawer, and then install it.

## Method 2: Adding SfNavigationDrawer reference from toolbox

Syncfusion also provides Xamarin Toolbox. Using this toolbox, you can drag the SfNavigationDrawer control to the XAML page. It will automatically install the required NuGet packages and add the namespace to the page. To install Syncfusion Xamarin Toolbox, refer to Toolbox.

## Method 3: Adding SfNavigationDrawer assemblies manually from the installed location

If you prefer to manually reference the assemblies instead referencing from NuGet, add the following assemblies in respective projects.

## Initialize SfNavigationDrawer
Import the SfNavigationDrawer namespace in respective Page as shown below:

**[XAML]**
```
<xmlns:navigationdrawer="clr-namespace:Syncfusion.SfNavigationDrawer.XForms;assembly=Syncfusion.SfNavigationDrawer.XForms"/>
```
**[C#]**
```
using Syncfusion.SfNavigationDrawer.XForms;
```
Then initialize an empty navigation drawer as shown below,

**[XAML]**
```
 <navigationdrawer:SfNavigationDrawer x:Name="navigationDrawer">
        <navigationdrawer:SfNavigationDrawer.ContentView>
            <Grid/>
        </navigationdrawer:SfNavigationDrawer.ContentView>
 </navigationdrawer:SfNavigationDrawer>
 ```
**[C#]**
```
public MainPage()
{
    InitializeComponent();
    SfNavigationDrawer navigationDrawer = new SfNavigationDrawer();
    Grid grid = new Grid();
    navigationDrawer.ContentView = grid;
    this.Content = navigationDrawer;
}
```
## How to run this application?

To run this application, you need to first clone the xamarin-forms-sfnavigationdrawer repository and then open it in Visual Studio 2022. Now, simply build and run your project to view the output.

## <a name="troubleshooting"></a>Troubleshooting ##
### Path too long exception
If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion has no liability for any damage or consequence that may arise by using or viewing the samples. The samples are for demonstrative purposes, and if you choose to use or access the samples, you agree to not hold Syncfusion liable, in any form, for any damage that is related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion’s samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion’s samples.