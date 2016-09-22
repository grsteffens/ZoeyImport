# ZoeyImport

This readme file talks about how to format CSV files so they can be imported into Zoey correctly.

<h3><i>Importing Products</i></h3>

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
        </ol>
      </li>
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
          <li>Not Taxable/ None = 1 (couldnt get to work)</li>
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

<hr>

<h3><i>Importing Images</i></h3>
<h4>In order to upload a csv file of images, the images must <a href="#mustExist">exist on the Zoey server first</a>.They need to be uploaded in yout control panel then you can use the links given to each image to include them in the csv file to associate each with their respective products.</h4>

Each CSV file used to import <b>images</b> should have 7 columns, each of which are described below:

<ol>

  <li>
    <b>sku</b>
    <ul>
      <li><b>This is a required attribute.</b> Without a SKU the images will not have a place to move to. This SKU must already be in your Products List, either through a CSV Upload or manual creation</li>
    </ul>
  </li>
  
  <li>
    <b>image</b>
    <ul>
      <li>This will be your Main Image, the main one that displays on the Products Page.</li>
    </ul>
  </li>
  
  <li>
    <b>small_image</b>
    <ul>
      <li>This should be the same value as your Main Image selection.</li>
    </ul>
  </li>
  
  <li>
    <b>thumbnail</b>
    <ul>
      <li>This should be the same value as your Main Image selection.</li>
    </ul>
  </li>
  
  <li>
    <b>_media_image (optional)</b>
    <ul>
      <li>Use this to assign multiple images to your product to show various views. These will appear as thumbnails on the Products Page</li>
    </ul>
  </li>
  
  <li>
    <b>_media_position (optional)</b>
    <ul>
      <li>Use this to assign positions to your additional images. 1 will show first, followed by 2, then 3 and so on.</li>
    </ul>
  </li>
  
  <li>
    <b>_media_is_disabled (optional)</b>
    <ul>
      <li>By the default this will be set to not-disabled (0). If you don't want to enable the image you can use this Header and enter 1 as a value.</li>
    </ul>
  </li>
  
</ol>

<a id="mustExist"></a><h4>In order to physically upload the image files, login to Zoey. Navigate to the left sidebar menu and go to Advanced > Import & Export. There, navigate to "Image Import" (the 5th row down) and select "Manage". Here, click "Upload Files" in the top right hand corner and select all files desired to be uploaded.</h4>
