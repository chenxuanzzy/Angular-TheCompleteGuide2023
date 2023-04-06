# Course 1 - Getting Started

  - [什麼是 Angular](#什麼是-angular)
  - [Angular vs Angular 2 vs Latest Angular Version](#angular-vs-angular-2-vs-latest-angular-version)
  - [安裝](#安裝)
  - [實作綁定 ngModel](#實作綁定-ngmodel)
  - [課程架構](#課程架構)
  - [補充](#補充)

## 什麼是 Angular

_Angular is a JavaScript Framework which allows you to create reactive [Single-Page-Applications(SPAs)](https://zh.wikipedia.org/zh-tw/%E5%8D%95%E9%A1%B5%E5%BA%94%E7%94%A8)._

## Angular vs Angular 2 vs Latest Angular Version

最初的 Angular 我們會稱 AngularJS 或 Angular 1 ，但後續更新的版本與現在差異甚大，Angular 團隊發現 AngularJS(Angular 1) 有太多的缺點(flaws)所以決定 Re-Write。在 2016 年 Angular 2 正式發行後與初版差異非常多，除非你有非常好的理由不然我們不會使用初版的做撰寫。後來因為某些原因跳過了 Angular 3 直接發行 4，漸漸的不停更新 5、6、7... 直到現在版本，我們皆統一稱為 Angular。

![image](https://user-images.githubusercontent.com/59633053/230306724-23d6de6a-f3e3-43b0-b745-4dc5ce6fe253.png)

## 安裝

[Angular.io](https://angular.io/guide/setup-local)

- `npm install -g @angular/cli@latest`
- `ng new my-dream-app`
- `cd my-dream-app`
- `ng serve`
  Angular Live Development Server _localhost:4200_

![image](https://user-images.githubusercontent.com/59633053/230323672-ecf78325-420e-42f6-b485-60f8522b8a79.png)

## 實作綁定 [ngModel](https://angular.io/api/forms/NgModel)

Angular CLI 生成出的檔案有這些

![image](https://user-images.githubusercontent.com/59633053/230328579-e3df2bb5-8f8c-4f05-a2db-5615d4618be0.png)

其中 app.component.ts 的 AppComponent 裡的 data 是綁定我們 html 的資料，當我修改 `name = 'Cindy'` 時，畫面 render 也會跟著改，這就是所謂的資料雙向綁定

![image](https://user-images.githubusercontent.com/59633053/230331378-6fa7180a-7f34-4323-b549-f9534212246d.png)

![image](https://user-images.githubusercontent.com/59633053/230329655-36745f9e-7aa6-4f9d-b809-4571786501af.png)

![image](https://user-images.githubusercontent.com/59633053/230331158-5864b4b2-63e2-49f6-8820-aab5115c360d.png)

這邊使用到 From 表單做雙向綁定，在 app.module.ts 中 `import { FormsModule } from '@angular/forms';` 一個內建套件
使用語法 `[(ngModel)]="name"`做綁定

![image](https://user-images.githubusercontent.com/59633053/230332264-8be77bde-26ed-4c42-a273-f15c5b626e9a.png)

![image](https://user-images.githubusercontent.com/59633053/230332743-04360f4a-24e4-41b6-822d-7435e7fd65d1.png)

簡單的實作就完成了

## 課程架構

![image](https://user-images.githubusercontent.com/59633053/230334675-86e438d6-10df-4750-a3c7-ec4ae8b0d542.png)

## 補充

![image](https://user-images.githubusercontent.com/59633053/230346114-d525c55c-daea-4d1f-a56f-ca1df83b266d.png)



課程資料來源 : [Angular - The Complete Guide(2023 Edition)](https://www.udemy.com/course/the-complete-guide-to-angular-2/)
