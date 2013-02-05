iOSWebView
==========

Simple ane to disable some native features of WebView:
 - disable manual scrolling the WebView, page panning is available
 - disable manual zooming with double tap and gesture touching

TODO:
 - allowing manual scrolling only vertically with native bounce effect
 - disabling background shadows and making background transparent

example:
Consts.IOS = Capabilities.manufacturer.indexOf("iOS") != -1;
if (Consts.IOS)
{
  var webview:StageWebView = new StageWebView();
  webview.stage = stage;
  webview.viewPort = new Rectangle(0, 0, stage.fulScreenWidth, stage.fullScreenHeight);
  
  WebView.instance.init();
  WebView.instance.setupWebView();
}
