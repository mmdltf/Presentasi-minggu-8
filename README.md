# Presentasi-minggu-8

# Presentasi Minggu 8 
# React-context dan React-testing

## React Context

React-context merupakan library built-in pada react js yang sebenar nya tidak dapat dibilang sebagai state management, namun ssalah satu kegunaan nya hmpir mirip dengan state management yang ada pada depedensi redux. Sama hal nya redux, react js menyediakan react-context untuk menyelesaikan persoalan props-drilling dimana kita harus mengirimkan props ke setiap komponen secara manual. Pengunaan react-context bisa dilakukan dengan cara React.createContext() sehingga data tersebuat bisa digunakan oleh komponen lain. Berikut cara penggunaan nya: 

    import React from "react"; 
    const UserContext = React.createContext(); 
    export default UserContext;
Dalam penggunaan react-context kita menggunakan 2 awal pada Tag yaitu  `Context.Provider` dan `Context.Consumer` dimana **context provider** digunakan untuk menyediakan data agar bisa di akses oleh komponen lainnya dan **context consumer** digunakan untuk mengakses data tersebut yang di sediakan oleh **context provider**. 

Contoh penggunakan nya: 
![enter image description here](https://i.postimg.cc/NfZW9gS9/image.png)




### React-context dengan Hooks
Dalam penggunaan react-context kita juga dapat memanfaatkan Hooks yaitu `useContext()` untuk mengakses data yang ada pada **Context provider**. Contoh penggunaan nya adalah seperti berikut:

![enter image description here](https://i.postimg.cc/PJMf2CDq/image.png)
## React Testing
Dalam sebuah project yang dilakukan oleh seseorang developer, pada akhirnya projec kita (sebuah website/ aplikasi ) akan di consume oleh orang lain, sebelum aplikasi yang kita buat akan digunakan oleh konsumer ada tahap yang harus dilalui selain proses develop yaitu testing. Proses ini berguna untuk mengetahui seberapa lancar nya performa aplikasi kita, ada banyak bug/ tidak, sudah layak di publish atau belum dan lainnya. Sebenarnya kita sudah biasa melakukan proses testing namun secara manual menggunakan console.log() ketika membuat sebuah logic. Namun terdapat library yang dapat digunakan untuk melakukan proses testing yaitu React Testing Library juga Jest.

Testing memilliki 3 tingkatan yaitu unit lalu integration dan end-to-end, dimana pada unit tes kita akan melakukan pengetesan pada bagian kecil. Setelah itu integration dimana kita melakukan pengetesan dari satu aplikasi yang terhubung (terintegrasi) ke aplikasi lain nya dan terakhir end-to-end dimana pengecekan dilakukan sampai tahap experience user. Ketika kita melakukan proese testing akan sering menemui test block dimana didalam nya terdapat beberapa bagian (render component, find element dan assert the result). Find element dapat menggunakan beberapa jenis (getBy, findBy, queryBy, getAllBy, findAllBy, quaeryAllBy)

 Ketika ingin melakukan pengetasan terdapat 2 jenis prosedur yaitu:

 -  membuat fitur lalu membuat testing.  
 -  membuat testing lalu
   membuat fitur, cara ini biasa disebut sebagai TDD dengan ciri
   red-zone, green-zone, blue-zone (refactor).
### Proses penginstallan
#### REACT TESTING LIBRARY

    npm install --save-dev @testing-library/react
    
    yarn add --dev @testing-library/react

#### JEST

    npm install --save-dev jest
    
    yarn add --dev jes




