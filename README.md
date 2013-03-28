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
