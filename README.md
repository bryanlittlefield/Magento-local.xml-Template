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
