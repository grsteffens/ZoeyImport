# ZoeyImport

This readme file talks about how to format CSV files so they can be imported into Zoey correctly.

Each CSV file used to import <b>products</b> should have 12 columns, each of which are described below:

<ol>

  <li>
    <b>sku</b>
    <ul>
      <li>A <b>unique</b> value to identify your product. No two products can share the same SKU.</li>
    </ul>
  </li>
  
  <li>
    <b>_type</b>
    <ul>
      <li>
        This is the type of product, there are 6 different types:
        <ol>
          <li>simple</li>
          <li>configurable</li>
          <li>group</li>
          <li>bundle</li>
          <li>virtual</li>
          <li>downloadable</li>
        </ol>
      </li>
      <li><a href="https://support.zoey.com/docs/product-types" target="_blank">More info on different types</a></li>
    </ul>
  </li>
  
  <li>
    <b>name</b>
    <ul>
      <li>The name of your product. By default this will also define the URL key and cannot be longer than 60 characters. <b>Name should always be UNIQUE. Having Duplicate Names causes SEO Issues.</b></li>
    </ul>
  </li>
  
  <li>
    <b>short_description</b>
    <ul>
      <li>A short description of your product found by the Add to Cart button.</li>
    </ul>
  </li>
  
  <li>
    <b>description</b>
    <ul>
      <li>A detailed description of your product.</li>
    </ul>
  </li>
  
  <li>
    <b>price</b>
    <ul>
      <li>The base price of the product, prior to any sales or discounts.</li>
    </ul>
  </li>
  
  <li>
    <b>status</b>
    <ul>
      <li>
        Whether or not to show this product in your store.
        <ol>
          <li>enabled = 1</li>
          <li>disabled = 2</li>
        </ol>
      </li>
    </ul>
  </li>
  
  <li>
    <b>tax_class_id</b>
    <ul>
      <li>
        Whether or not to charge tax for this product.
        <ol>
          <li>Not Taxable/ None = 1</li>
          <li>Taxable = 2</li>
        </ol>
      </li>
    </ul>
  </li>
  
  <li>
    <b>visibility</b>
    <ul>
      <li>
        How your customers can find this product.
        <ol>
          <li>Not Visible Individually = 1</li>
          <li>Catalog Only = 2</li>
          <li>Search Only = 3</li>
          <li>Catalog and Search = 4</li>
        </ol>
      </li>
    </ul>
  </li>
  
  <li>
    <b>weight</b>
    <ul>
      <li>The weight of your product expressed only as a number.</li>
    </ul>
  </li>
  
  <li>
    <b>qty</b>
    <ul>
      <li>Quantity available to purchase</li>
    </ul>
  </li>
  
  <li>
    <b>is_in_stock</b>
    <ul>
      <li>
        If this product is in-stock or not.
        <ol>
          <li>1 = In Stock</li>
          <li>0 = Out of Stock</li>
        </ol>
      </li>
    </ul>
  </li>
  
</ol>
