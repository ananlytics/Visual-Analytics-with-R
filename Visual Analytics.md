## Visual-Analytics-with-R
# A picture is worth a 1000 words; unless you are working with Big data in which case it is worth millions.

1. Plotting temperature distribution. Bigger and denser the polygon, more the corresponding no. of records. Plotting polygons with no color variation can fail to generate required insights. Hence, good choice would be to add multiple colors or do what I have tried in below graph.
```

ggplot(df, aes(x=y,y=temp))+geom_polygon(aes(alpha = 50))

```
![11](https://user-images.githubusercontent.com/104814594/166864895-8642e82f-17cb-4c31-a206-747d54e89352.JPG)

2. As above plot is hard to interpret. Following density plot gives better interpretation. 

```
ggplot(df, aes(x=y,y=temp))+geom_hex(color='blue')

```

![12](https://user-images.githubusercontent.com/104814594/166865687-c7d7739f-d504-4722-8423-cda72841781c.JPG)
