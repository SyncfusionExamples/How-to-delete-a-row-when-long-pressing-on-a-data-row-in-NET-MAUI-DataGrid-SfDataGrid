# How to delete a row when long pressing on a data row in .NET MAUI DataGrid SfDataGrid
The [.NET MAUI DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid) allows you to delete a row by performing a long press on a data row and hooking into the [SfDataGrid.CellLongPress](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.DataGrid.SfDataGrid.html#Syncfusion_Maui_DataGrid_SfDataGrid_CellLongPress) event.

Refer to the code example below, where the SfDataGrid is grouped by a column, and the CellLongPress event is hooked.

##### Xaml
 
 ```XML
<syncfusion:SfDataGrid ColumnWidthMode="Auto"
                           ItemsSource="{Binding Employees}"
                           CellLongPress="datagrid_CellLongPress">
</syncfusion:SfDataGrid>
 ```
 
The following code illustrates how to delete a row in the SfDataGrid by performing a long press on it.
##### C#
 
 ```XML
private void datagrid_CellLongPress(object sender, DataGridCellLongPressEventArgs e)
{
    viewModel.Employees.Remove((Employee)e.RowData);
}
 ```
 

[View sample in GitHub](https://github.com/SyncfusionExamples/How-to-delete-a-row-when-long-pressing-on-a-data-row-in-NET-MAUI-DataGrid-SfDataGrid/tree/859172)

Take a moment to explore this [documentation](https://help.syncfusion.com/maui/datagrid/overview), where you can find more information about Syncfusion .NET MAUI DataGrid (SfDataGrid) with code examples. Please refer to this [link](https://www.syncfusion.com/maui-controls/maui-datagrid) to learn about the essential features of Syncfusion .NET MAUI DataGrid (SfDataGrid).

##### Conclusion

I hope you enjoyed learning about how to delete a row when long pressing on a data row in .NET MAUI DataGrid(SfDataGrid).

You can refer to our [.NET MAUI DataGrid’s feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to learn about its other groundbreaking feature representations. You can also explore our .NET MAUI DataGrid Documentation to understand how to present and manipulate data. For current customers, you can check out our .NET MAUI components on the [License and Downloads](https://www.syncfusion.com/account/downloads) page. If you are new to Syncfusion, you can try our 30-day free trial to explore our .NET MAUI DataGrid and other .NET MAUI components. If you have any queries or require clarifications, please let us know in the comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/account/login?ReturnUrl=%2Faccount%2Fconnect%2Fauthorize%2Fcallback%3Fclient_id%3Dc54e52f3eb3cde0c3f20474f1bc179ed%26redirect_uri%3Dhttps%253A%252F%252Fsupport.syncfusion.com%252Fagent%252Flogincallback%26response_type%3Dcode%26scope%3Dopenid%2520profile%2520agent.api%2520integration.api%2520offline_access%2520kb.api%26state%3D8db41f98953a4d9ba40407b150ad4cf2%26code_challenge%3DvwHoT64z2h21eP_A9g7JWtr3vp3iPrvSjfh5hN5C7IE%26code_challenge_method%3DS256%26response_mode%3Dquery) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid), or the feedback portal. We are always happy to assist you!
