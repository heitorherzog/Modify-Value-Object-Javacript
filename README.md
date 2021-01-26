#Change object value by passing the path structure
Find the property in a nest object, change the value and returnig the object modified 

### object that will be modified
```javascript
 const obj = {
      aProperty: {
        aSetting1: 1,
        aSetting2: 2,
        aSetting3: 3,
        aSetting4: 4,
        aSetting5: 5,
      },
      bProperty: {
        bSetting1: {
          bPropertySubSetting: true,
          dPropertySubSetting: {
            dProperty: {
              dSetting1: 11,
              dSetting2: 22,
              dSetting3: 33,
              dSetting4: 44,
              dSetting5: 55,
            },
          },
        },
        bSetting2: "bString",
      },
      cProperty: {
        cSetting: "cString",
      },
    };
```
### dSetting1 value  will be change to 11 to 1000

```javascript
 SetValue(
      obj,
      "bProperty.bSetting1.dPropertySubSetting.dProperty.dSetting1",
      1000
    );
 ```
    
  
