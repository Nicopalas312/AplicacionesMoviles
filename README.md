# AplicacionesMoviles Eduardo Palacio
Maquinaria Arriendo
Para abrir el proyecto:
npm i ,
npm install -g @angular/cli ,
ionic s ,


Para instalar android Studio:

npm install @capacitor/android ,
npx cap add android ,
Ionic build Android ,

ionic capacitor sync android ,

Para iniciar android Studio:

npx cap open android ,


opcional:
esto es para el dark mode ,
npm install @capacitor/preferences ,
npx cap sync,


para el pc de la profe:
npm.cmd i -D -E @angular/cli

13- Diríjase a su proyecto en visual y diríjase a la ubicación del archivo “barcodescanner.gradle”,el cual se encuentra 
en la siguiente ruta:node_modules/phonegap-plugin-barcodescanner/src/android/barcodescanner.gradle
14- En el archivo cambiar en la dependencia compile por implementation como se muestra acontinuación este error ya se encuentra solucionado

dependencies {
compile(name:'barcodescanner-release-2.1.5', ext:'aar')
}

dependencies 
{implementation(name:'barcodescanner-release-2.1.5', ext:'aar')
}

17- Dirigirse nuevamente a su proyecto y diríjase a la siguiente ubicación del archivo:"android/gradle.properties"
Y agregar lo siguiente:
android.useAndroidX=true
android.enableJetifier=true
