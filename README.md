Magento-local.xml-Template
==========================

A great Start for your next Magento Theme's local.xml file


```xml
<?xml version="1.0"?>
<layout>
  
<!--
Add/Remove Items From Head
-->
  <default translate="label" module="page">
    <reference name="head">
      <!-- Add Javascript File -->
      <action method="addJs"><script>jquery/jquery.js</script></action>
      <!-- Add CSS File -->
      <action method="addCss"><stylesheet>css/local.css</stylesheet></action>
    </reference>
  </default>

<!--
Default layout, loads most of the pages
-->
  <default>
    <!-- Header -->
    <reference name="header">
      <!-- Insert Code Here -->
    </reference>

    <!-- Left Sidebar -->
    <reference name="left"> 
      <!-- Insert Code Here -->
    </reference> 

    <!-- Right Sidebar -->
    <reference name="right">
       <remove name="right.poll" />
    </reference>

    <!-- Content -->
    <reference name="content">
      <!-- Insert Code Here -->
    </reference>

    <!-- Top Nav -->
    <reference name="top.nav">
      <!-- Insert Code Here -->
    </reference>

  </default>

<!--
CMS Layout
-->
  <cms_page>

    <!-- Header -->
    <reference name="header">
      <!-- Insert Code Here -->
    </reference>

    <!-- Left Sidebar -->
    <reference name="left"> 
      <!-- Insert Code Here -->
    </reference> 

    <!-- Right Sidebar -->
    <reference name="right">
      <!-- Insert Code Here -->
    </reference>

    <!-- Content -->
    <reference name="content">
      <!-- Insert Code Here -->
    </reference>

  </cms_page>

<!--
CMS Homepage
-->
  <cms_index_index>

    <!-- Header -->
    <reference name="header">
      <!-- Insert Code Here -->
    </reference>

    <!-- Left Sidebar -->
    <reference name="left"> 
      <!-- Insert Code Here -->
    </reference> 

    <!-- Right Sidebar -->
    <reference name="right">
      <!-- Insert Code Here -->
    </reference>

    <!-- Content -->
    <reference name="content">
      <!-- Insert Code Here -->
    </reference>

  <cms_index_index>



<!--
Catalog Category Layout
-->
  <catalog_category_default translate="label">
    <!-- Insert Code Here -->
  </catalog_category_default>  

<!--
Catalog Product View Layout
-->
  <catalog_product_view translate="label">
    <!-- Insert Code Here -->
  </catalog_product_view>  

<!--
Catalog Layered Layout
-->
   <catalog_category_layered translate="label">
    <!-- Insert Code Here -->
   </catalog_category_layered>

<!--
Catalog Search Results Layout
-->
  <catalogsearch_result_index translate="label">
    <!-- Insert Code Here -->
  </catalogsearch_result_index>

<!--
Catalog Advanced Search Layout
-->
  <catalogsearch_advanced_index translate="label">
    <!-- Insert Code Here -->
  </catalogsearch_advanced_index>  

<!--
Catalog Advanced Search Results Layout
-->
  <catalogsearch_advanced_result translate="label">
    <!-- Insert Code Here -->
  </catalogsearch_advanced_result>  

<!--
Cart Template
-->
  <checkout_cart_index translate="label">
   <!-- Insert Code Here -->
  </checkout_cart_index>

<!--
Checkout Layout
-->
  <checkout_onepage_index>
   <!-- Insert Code Here -->
  </checkout_onepage_index>

<!--
Contact Page Template
-->
  <contacts_index_index translate="label">
    <!-- Insert Code Here -->
  </contacts_index_index>

<!--
Customer Account Layout
-->
  <customer_account>
    <!-- Insert Code Here -->
  </customer_account>

<!--
Customer Account
-->
  <customer_account>
  <!-- Insert Code Here -->  
  </customer_account>

<!--
Customer Login Page
-->
  <customer_account_login>
  <!-- Insert Code Here -->  
  </customer_account_login>

<!--
Customer Forgot Password
-->
  <customer_account_forgotpassword>
  <!-- Insert Code Here -->  
  </customer_account_forgotpassword>

<!--
Customer Logged In
-->
  <customer_logged_in>
    <!-- Insert Code Here -->
  </customer_logged_in>

<!--
Customer Logged Out
-->
  <customer_logged_out>
    <!-- Insert Code Here -->
  </customer_logged_out>

</layout>

<!-- List of Usefull Removals
    <remove name="catalog.compare.sidebar" />
    <remove name="right.permanent.callout" />
    <remove name="left.permanent.callout" />
    <remove name="left.newsletter" />
    <remove name="right.reports.product.viewed" />
    <remove name="paypal.partner.right.logo" />
    <remove name="right.poll" />
    <remove name="cart_sidebar" />
    <remove name="checkout_cart_link" />
    <remove name="catalog.compare.list" /> -->


```
Available layout xml handles
==============================

```xml
default
catalog_category_default    (* also used in directory.xml)
catalog_category_layered    (* also used in directory.xml)
catalog_product_compare_index
catalog_product_gallery
catalog_product_send
catalog_product_view   (* also used in customeralert.xml, tag.xml)
catalog_seo_searchterm_popular
catalog_seo_sitemap_category
catalog_seo_sitemap_product

catalogsearch_advanced_form
catalogsearch_advanced_result
catalogsearch_result_index
catalogsearch_term_popular

checkout_cart_index      (* also used in googlecheckout.xml, paypal.xml)
checkout_multishipping
checkout_multishipping_address_editaddress
checkout_multishipping_address_editbilling
checkout_multishipping_address_editshipping
checkout_multishipping_address_newbilling
checkout_multishipping_address_newshipping
checkout_multishipping_address_select
checkout_multishipping_address_selectbilling
checkout_multishipping_addresses
checkout_multishipping_billing
checkout_multishipping_customer_address
checkout_multishipping_login
checkout_multishipping_overview
checkout_multishipping_register
checkout_multishipping_shipping
checkout_multishipping_success
checkout_onepage_additional
checkout_onepage_index
checkout_onepage_progress
checkout_onepage_review
checkout_onepage_shippingmethod
checkout_onepage_success

cms_index_defaultindex
cms_index_defaultnoroute


customer_account            (* also used in newsletter.xml, review.xml, sales.xml, wishlist.xml)
customer_account_create
customer_account_edit
customer_account_forgotpassword
customer_account_index      (* also used in catalog.xml, newsletter.xml, poll.xml, review.xml, sales.xml, tag.xml, wishlist.xml)
customer_account_login
customer_address_form
customer_address_index
customer_logged_in
customer_logged_out
customer_account_logoutsuccess

giftmessage_index_edit
giftmessage_index_save
giftmessage_index_remove

newsletter_manage_index

paypal_express_review
paypal_express_review_details

print

review_customer_index
review_customer_view
review_product_list
review_product_view
reviews

sales_order_details
sales_order_history
sales_order_print
sales_order_view

shipping_tracking_ajax

tag_customer_index
tag_customer_edit
tag_customer_view
tag_list_index

wishlist_index_index
```


Available Attributes
==============================

```xml
addPriceBlockType:   <action method="addPriceBlockType"><type>bundle</type><block>bundle/catalog_product_price</block><template>bundle/catalog/product/price.phtml</template></action>

addItemRender:   <action method="addItemRender"><type>bundle</type><block>
bundle/checkout_cart_item_renderer</block><template>checkout/cart/sidebar/default.phtml</template></action>

addItem: <action method="addItem"><type>skin_js</type><name>js/bundle.js</name></action>
insert: <action method="insert"><block>product.info.bundle.options</block></action>

setItemLimit: <action method="setItemLimit"><type>bundle</type><limit>4</limit></action>

setImgSrc: <action method="setImgSrc"><src>images/media/col_left_callout.jpg</src></action>

setImgAlt: <action method="setImgAlt" translate="alt" module="catalog"><alt>Our customer service is available 24/7. Call us at (800) DEMO-NUMBER.</alt></action>

setLinkUrl: <action method="setLinkUrl"><url>checkout/cart</url></action>

addLink:   <action method="addLink" translate="label title" module="catalog" ifconfig="catalog/seo/site_map"><label>Site Map</label><url helper="catalog/map/getCategoryUrl" /><title>Site Map</title></action>

setDefaultListPerPage: <action method="setDefaultListPerPage"><limit>4</limit></action>

setDefaultGridPerPage: <action method="setDefaultGridPerPage"><limit>9</limit></action>

addPagerLimit: <action method="addPagerLimit"><mode>list</mode><limit>6</limit></action>

setToolbarBlockName: <action method="setToolbarBlockName"><name>product_list_toolbar</name></action>

addReviewSummaryTemplate: <action method="addReviewSummaryTemplate"><type>default</type><template>review/helper/su.phtml</template></action>

setTemplate: <action method="setTemplate"><template>page/one-column.phtml</template></action>

addJs: <action method="addJs"><script>scriptaculous/scriptaculous.js</script></action>

unsetChild: <action method="unsetChild"><name>catalog_compare_sidebar</name></action>

setTierPriceTemplate: <action method="setTierPriceTemplate"><template>catalog/product/view/tierprices.phtml</template></action>

setColumnCount: <action method="setColumnCount"><columns>4</columns></action>

setItemLimit: <action method="setItemLimit"><type>upsell</type><limit>4</limit></action>

addOptionRenderer: <action method="addOptionRenderer"><type>text</type><block>catalog/product_view_options_type_text</block><template>catalog/product/view/options/type/text.phtml</template></action>

insert: <action method="insert"><block>product.tierprices</block></action>

append: <action method="append"><block>product.info.addtocart</block></action>

setDataByKey: <action method="setDataByKey"><key>alias_in_layout</key><value>container2</value></action>

setDataByKeyFromRegistry: <action method="setDataByKeyFromRegistry"><key>options_container</key><key_in_registry>product</key_in_registry></action>

unsetCallChild: <action method="unsetCallChild"><child>container1</child><call>ifEquals</call><if>0</if><key>alias_in_layout</key><key>options_container</key></action>

setTitle: <action method="setTitle" translate="title" module="catalog"><title>Categories</title></action>

bindPager: <action method="bindPager"><pager>seo.sitemap.pager.top</pager></action>

setItemsTitle: <action method="setItemsTitle" translate="title" module="catalog"><title>categories</title></action>

setListOrders: <action method="setListOrders"/>

setListModes: <action method="setListModes"/>

setListCollection: <action method="setListCollection"/>

addCartLink: <action method="addCartLink"></action>

addCheckoutLink: <action method="addCheckoutLink"></action>

setCartTemplate: <action method="setCartTemplate"><value>checkout/cart.phtml</value></action>

setEmptyTemplate: <action method="setEmptyTemplate"><value>checkout/cart/noItems.phtml</value></action>

chooseTemplate: <action method="chooseTemplate"/>

setMethodFormTemplate: <action method="setMethodFormTemplate"><method>purchaseorder</method><template>payment/form/purchaseorder.phtml</template></action>

setInfoTemplate: <action method="setInfoTemplate"><method></method><template></template></action>

setDontDisplayContainer: <action method="setDontDisplayContainer"><param>1</param></action>

setBlockId: <action method="setBlockId"><block_id>footer_links</block_id></action>

setHeaderTitle: <action method="setHeaderTitle" translate="title" module="contacts"><title>Contact Us</title></action>

setSaveMode: <action method="setSaveMode"><mode>save</mode></action>

setGoogleCheckout: <action method="setGoogleCheckout"><flag>true</flag></action>

setScriptType: <action method="setScriptType"><scriptType>control_script</scriptType></action>

addCss: <action method="addCss"><stylesheet>css/reset.css</stylesheet></action>

setPollTemplate: <action method="setPollTemplate"><template>poll/active.phtml</template><type>poll</type></action>

addWishlistLink: <action method="addWishlistLink"></action>
```


