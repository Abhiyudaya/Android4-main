Fixes :
1 . Collecting data returned by the fetchResults() function in a <List<CimputerItem>> named _listStringData which is a MutableStateFlow and then using the data to expose a StateFlow for the UI.

2 . changes in JarRepository for emitting data in the fetchResults function for the StateFlow to collect in the ViewModel.

3 . Changing visibility by changing text color from Transparent to Black  (read it in a blog)

4 . Wasn't able to return from second screen to first screen because navigate.value was not set to ""
        so i changed it's value back to "" once the navigation is done.

Implementation :
SearchQuery implementation by filtering out from the original api data and then showing it using a LazyColumn.
