var dic = ee.Dictionary({
  "name":"Rahi",

  "hobby":"Illustratiting",

  "numList":[2,3,4,5,6,7,9]
})
print(dic.get("name"))
print(dic.get("hobby"))
print(dic.get("numList"))

var numList = ee.List([2,3,4,5,6,7,9])
print("List of the number: ", numList)

var sumNum = numList.reduce(ee.Reducer.sum())
print("Sum of the number is: ", sumNum)
