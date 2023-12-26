# swiperslider
Swiper Slider Development by Dilawar khan In Angular
 # Create Project in Angular:
  ng new Project
  
 # Directory to your Project:
  cd Project
  
 # Swiper Install in to your Project:
  npm install swiper

  
 # App.modules.ts Modified:
  
import { CUSTOM_ELEMENTS_SCHEMA, NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';

// import function to register Swiper custom elements
import { register } from 'swiper/element/bundle';
// register Swiper custom elements
register();


@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent],

  schemas: [CUSTOM_ELEMENTS_SCHEMA]
})
export class AppModule { }


  
 # App.component.html Modified:
  
<swiper-container
  navigation="true"
  pagination="true"
  pagination-clickable="true" 
  >
  <swiper-slide>
    <img class="img_custom" src="/assets/sliders1.png" alt="">
  </swiper-slide>
  <swiper-slide>
    <img class="img_custom" src="/assets/sliders2.png" alt="">

  </swiper-slide>
  <swiper-slide>
    <img class="img_custom" src="/assets/sliders3.png" alt="">

  </swiper-slide>
</swiper-container>

# Run Project:
  ng serve

