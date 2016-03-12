Time-of-flight inflow angiography
*********************************

:status: hidden
:slug: mod_angio
:JavaScripts: papaya.js
:Stylesheets: papaya.css

**Arteriography**

In time-of-flight angiography image flowing blood, such as the one in arteries,
appears much brighter than stationary brain tissue.  The sample image below is
a low-resolution demo of the actual angiographies in the dataset.
`More information on this image type 
<http://en.wikipedia.org/wiki/Magnetic_resonance_angiography>`_.

.. raw:: html

  <script type="text/javascript">
      var params = [];
      params["worldSpace"] = false;
      params["images"] = ["/data/angio.nii.gz"];
      params["expandable"] = true;
      params["kioskMode"] = true;
      params["angio.nii.gz"] = {"min": 0, "max": 150};
  </script>

  <div class="row">
    <div class="col-md-12">
      <div class="papaya-preview" data-params="params">
        <img class="img-responsive"
             src="/pics/mod_angio_viewer_preview.jpg"
             title="Click to load interactive viewer"
             alt="Angiography example image"
             onclick="$(this.parentNode).addClass('papaya'); papaya.Container.startPapaya(); this.parentNode.removeChild(this);" />
      </div>
    </div><!-- /.col-md-12 -->
  </div><!-- /.row -->

Technical details
=================

Volumetric images (640x480x150) in NIfTI format recorded with a Siemens MR
scanner at 7 Tesla using a 3D multi-slab sequence (0.3 mm isotropic voxel
size). These images have partial brain coverage |---| approximately the same
volume as the functional MRI scans.

.. |---| unicode:: U+02014 .. em dash