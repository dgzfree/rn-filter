install
--------
npm i filter-dugz  
npm i utilities-dugz  
npm install --registry=http://cnpm.58v5.cn/

------
base usage
----
```javascript
 <NewFilterView filterInfo={this.listState.filterInfo}
      // showFilterTitle={false}
      //                     animType={"popUp"}
                          // dialogHeight={ListConstants.NEW_FILTER_DIALOG_HEIGHT}
                          // titleHeight={ListConstants.NEW_FILTER_VIEW_HEIGHT}
                          bgHeight={Utilities.viewMaxHeight - ListConstants.NAVIGATION_VIEW_HEIGHT - ListConstants.NEW_FILTER_VIEW_HEIGHT}
      //                     colorStyle={{
      //                       "defaultFontColor": "pink",
      //                       "defaultBgColor": "skyblue",
      //                       "selectedFontColor": "lightyellow",
      //                       "selectedBgColor": "lightgrey",
      //                       "defaultImg": FilterConstants.DEFAULT_IMG,
      //                       "defaultSelectedImg": FilterConstants.DEFAULT_SELECTED_IMG,
      //                       "selectedImg": FilterConstants.SELECTED_IMG,
      //                       "parentListSelectedBgColor": FilterConstants.PARENT_LIST_SELECTED_BD_COLOR,
      //                       "parentListSelectedImg": FilterConstants.PARENT_LIST_SELECTED_IMG,
      //                       "childListSelectedImg": FilterConstants.CHILD_LIST_SELECTED_IMG,
      //                       "delSelectedImg": FilterConstants.DEL_SELECTED_IMG,
      //                       "borderRadius": FilterConstants.BORDER_RADIUS,
      //                       "submitBgColor": FilterConstants.SUBMIT_BG_COLOR,
      //                       "childSelectedBottomRightImg": FilterConstants.CHILD_SELECTED_BOTTOM_RIGHT_IMG
      //                     }}
      //                     typeMultiLevelParams={{ "showReset": true, "minSelect": 2 }}
                          callback={this.onNewFilterViewCallback}
                          productId = {1}
                          sceneId = {1}
                          cate={String(global.jumperParams.content.params.full_path)}
    />;
```
--------
API
-----
```javascript
    static propTypes = {
    filterInfo: PropTypes.object.isRequired,
    showFilterTitle: PropTypes.bool,
    callback: PropTypes.func.isRequired,
    cate: PropTypes.string.isRequired,
    animType: PropTypes.string,
    colorStyle: PropTypes.object,
    dialogHeight: PropTypes.number,
    animDuring: PropTypes.number,
    typeMultiLevelParams: PropTypes.object,
    bgHeight: PropTypes.number,
    titleHeight: PropTypes.number,
    productId: PropTypes.number.isRequired,
    sceneId: PropTypes.number.isRequired
  };

  static defaultProps = {
    dialogHeight: 400,
    bgHeight: Utilities.viewMaxHeight,
    animDuring: 300,
    titleHeight: 45,
    showFilterTitle: true,
    animType: "drop",
    typeMultiLevelParams: {
      "showReset": false,
      "minSelect": 0,
      "requestUrl": "http://socialhouse.58.com/api/partner/local/api_get_local"
    },
    colorStyle: {
      "defaultFontColor": FilterConstants.DEFAULT_FONT_COLOR,
      "defaultBgColor": FilterConstants.DEFAULT_BG_COLOR,
      "selectedFontColor": FilterConstants.SELECTED_FONT_COLOR,
      "selectedBgColor": FilterConstants.SELECTED_BG_COLOR,
      "defaultImg": FilterConstants.DEFAULT_IMG,
      "defaultSelectedImg": FilterConstants.DEFAULT_SELECTED_IMG,
      "selectedImg": FilterConstants.SELECTED_IMG,
      "parentListSelectedBgColor": FilterConstants.PARENT_LIST_SELECTED_BD_COLOR,
      "parentListSelectedImg": FilterConstants.PARENT_LIST_SELECTED_IMG,
      "childListSelectedImg": FilterConstants.CHILD_LIST_SELECTED_IMG,
      "delSelectedImg": FilterConstants.DEL_SELECTED_IMG,
      "borderRadius": FilterConstants.BORDER_RADIUS,
      "submitBgColor": FilterConstants.SUBMIT_BG_COLOR,
      "childSelectedBottomRightImg": FilterConstants.CHILD_SELECTED_BOTTOM_RIGHT_IMG
      "defaultBgColorGrey": FilterConstants.DEFAULT_BG_COLOR_GREY,
    }
  };
  
 ```
