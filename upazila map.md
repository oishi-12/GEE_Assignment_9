var bgd = ee.FeatureCollection("projects/ee-oishirahi9865/assets/BGD_adm3");
print(bgd.aggregate_array("NAME_3"))

var upazilla = bgd.filter(ee.Filter.eq("NAME_3","Hathazari")).geometry().area()
print(upazilla)
var upazilla = bgd.filter(ee.Filter.eq("NAME_3","Hathazari"))
Map.centerObject(upazilla, 11) 
Map.addLayer(upazilla,{},"Hathazari")
