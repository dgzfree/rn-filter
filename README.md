# rn-filter

install

npm i dgz-rn-filter

data

http://c.58corp.com/pages/viewpage.action?pageId=19059154#id-%E3%80%90%E6%89%BE%E5%AE%A4%E5%8F%8B%E3%80%91%E6%8E%A5%E5%8F%A3API-%E5%B8%96%E5%AD%90%E5%85%AC%E5%85%B1%E5%88%97%E8%A1%A8%E6%8E%A5%E5%8F%A3%EF%BC%88%E6%9F%A5%E4%BA%91%E6%90%9C%EF%BC%89

API

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
