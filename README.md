# Thesis
* For power grid models, a corresponding GLM file needs to be placed
  in the `GLM/` directory in order to make topology visualization
  possible.
* For network devices, after adding a new device into the database the
  file `Scripts/NetGen.py` needs to be edited to make sure that the
  new device is integrated with the built-in network model.
* The built-in network model cannot be changed without modifying the
  source code; this filed needs to be edited
  `Scripts/NetGen.py` mentioned above.
