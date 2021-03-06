---
-api-id: E:Windows.Storage.Search.StorageFileQueryResult.ContentsChanged
-api-type: winrt event
---

<!-- Event syntax
public event Windows.Foundation.TypedEventHandler ContentsChanged<Windows.Storage.Search.IStorageQueryResultBase,  object>
-->

# Windows.Storage.Search.StorageFileQueryResult.ContentsChanged

## -description
Fires when a file is added to, deleted from, or modified in the folder being queried. This event only fires after [GetFilesAsync](storagefilequeryresult_getfilesasync.md) has been called at least once.

## -remarks
If you register a handler for this event, keep that handler registered while you suspend your app (in response to [oncheckpoint](http://msdn.microsoft.com/library/a7620c81-f769-46e5-b030-dde21b8c2d5b) or [Suspending](../windows.ui.xaml/application_suspending.md)). Your app will not receive [ContentsChanged](storagefilequeryresult_contentschanged.md) events while it is suspended and when your app resumes it will receive a single event that aggregates all of the changes if any occurred.

Additionally, keep in mind that registering and removing event handlers are synchronous operations and might cause your app to stop responding briefly if you execute them on your app's UI thread. Wherever possible, use a thread other than your app's UI thread to register and unregister these event handlers.

## -examples

## -see-also
