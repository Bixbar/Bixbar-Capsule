# Bixbar-Capsule

## Directory structure
- 📁 assets
  - 📁 images
- 📁 code
  - findbyCocktailName.js
  - findbyBaseSpirit.js  
  - findbyBaseClick.js
  - recommandFood.js
  - CreateUser.js
  - submitSurvey.js
  - findGender.js
  - Personalize.js
  - PersonalClick.js
- 📁 models
  - 📁 actions
  - 📁 concepts
    - 📁 Input
    - 📁 OutputInfos
    - 📁 ResultStructure
- 📁 resources
  - 📁 Base
    - 📁 layouts
      - CocktailList.layout.bxb
      - CocktailDetail.layout.bxb
    - 📁 views
      - CocktailResult.view.bxb
      - BaseSpiritResults.view.bxb
      - BaseClickResult.view.bxb
      - FoodResults.view.bxb
      - UserInfo.view.bxb
      - Age_Input.view.bxb
      - Geder_Input.view.bxb
      - Personal.view.bxb
      - PerClickResult.view.bxb
    - capsule.properties
    - endpoints.bxb

## Code reivew
### $vivContext.bixbyUserId
```javascript
user = {
    "gender": "Male",
    "age": survey.age,
    "userID" : $vivContext.bixbyUserId,
    };
```
- `$vivContext` : 사용자 컨텍스트를 표시한다.
  - 이를 통하여 bixbyUserId에 접근한다.

```bixby
capsule {
  permissions {
    bixby-user-id-access
  }
}
```
- 엑세스하기 위해서는 bixby-user-id-access에 대한 퍼미션을 설정해야 한다.
