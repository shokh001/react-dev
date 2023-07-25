# react-dev
1. **React nima?**
React - bu bitta sahifali ilovalar uchun foydalanuvchi interfeyslarini ishlab chiqishda foydali bo'lgan front-end va ochiq manbali JavaScript kutubxonasi.

2. **Reactning muhim xususiyatlari quyidagilardir:**
   * U server tomonida renderlashni qo'llab-quvvatlaydi.
   * RealDOM manipulyatsiyasi qimmat bo'lgani uchun u haqiqiy DOM (Data Object Model) o'rniga virtual DOM dan foydalanadi.
   * U bir tomonlama ma'lumotlarni ulash yoki ma'lumotlar oqimini kuzatib boradi.
   * Ko'rinishni ishlab chiqish uchun qayta foydalanish mumkin yoki birlashtirilishi mumkin bo'lgan UI komponentlaridan foydalanadi.

3. React to'liq ishlab chiqilgan ramka emas, chunki u faqat kutubxona.

4. **Kalitlarning ahamiyati:**
   * Kalitlar qaysi elementlar qo'shilgan, o'zgartirilgan yoki o'chirilganligini aniqlashga yordam beradi.
   * Har bir element uchun noyob identifikatsiyani ta'minlash uchun massiv elementlariga kalitlar berilishi kerak.
   * Kalitlarsiz React har bir elementning tartibini yoki o'ziga xosligini tushunmaydi.
   * Kalitlar yordamida React qaysi element o'chirilgan, tahrirlangan va qo'shilganligi haqida fikrga ega.
   * Kalitlar odatda API dan keladigan ma'lumotlar ro'yxatini ko'rsatish uchun ishlatiladi.

5. **JSX nima?**
   * JSX JavaScript XML degan ma'noni anglatadi. Bu bizga HTML-ni JavaScript-da yozish va ularni DOM-ga appendChild( ) yoki createElement( ) kabi funksiyalardan foydalanmasdan joylashtirish imkonini beradi.
   * React rasmiy hujjatlarida aytilganidek, JSX React.createElement( ) funksiyasi uchun sintaktik shakarni taqdim etadi.

6.  **Virtual DOM** - bu haqiqiy DOMning virtual ko'rinishi xotirada saqlanadigan va ReactDOM kabi kutubxona tomonidan haqiqiy DOM bilan sinxronlashtirilgan tushunchadir.

7.  **React Hooks nima?**
React Hooks - bu ishlab chiquvchilarga React komponentlarida holat va hayot aylanish usullaridan foydalanishga ruxsat beruvchi o'rnatilgan funktsiyalar. Bular React 16.8 versiyasida taqdim etilgan yangi qo'shilgan funksiyalardir.

8. StrictMode - bu ilovadagi mumkin bo'lgan muammolarni ta'kidlash uchun Reactning 16.3 versiyasiga qo'shilgan vosita . U ilovada qo'shimcha tekshiruvlarni amalga oshiradi.

9. **React-da re-render sababi:**
   * Komponent va uning yordamchi komponentlarini re-render qilish props yoki state o'zgartirilganda sodir bo'ladi.
   * Yangilanmagan komponentlarni re-render qilish ilovaning ishlashiga ta'sir qiladi.

10. Oddiy qilib aytganda, Higher-Order Component (HOC) - bu komponentni qabul qiladigan va yangi komponentni qaytaradigan funksiya. 

11. **State va Props farqi:** 
   * **State** - Komponent o'rnatilganda standart qiymatdan boshlanadigan ma'lumotlar strukturasi. U vaqt o'tishi bilan, asosan foydalanuvchi hodisalari natijasida mutatsiyaga uchragan bo'lishi mumkin.

   * **Props** (xususiyatlarning qisqartmasi) Komponent konfiguratsiyasidir. Ular yuqoridan qabul qilinadi va ularni qabul qiluvchi komponentga nisbatan o'zgarmasdir. Komponent o'z Propsini o'zgartira olmaydi, lekin u o'zining asosiy komponentlarining Propsini birlashtirish uchun javobgardir. Callback funktsiyalari props sifatida ham o'tkazilishi mumkin.

12. **Turli xil lifecycle methodlari nima?**
   * **componentWillMount (deprecated)** - bu ildiz komponentingizda ilovalarni sozlash uchun eng ko'p ishlatiladi.
   * **componentDidMount** - bu erda siz DOMsiz qila olmagan barcha sozlashlarni amalga oshirmoqchisiz va kerakli ma'lumotlarni olishni boshlaysiz. Bundan tashqari, agar siz eventListeners va hokazolarni o'rnatmoqchi bo'lsangiz, bu hayot aylanishi kancasi buni amalga oshirish uchun yaxshi joy.
   * **componentWillReceiveProps (deprecated)** - bu hayot tsikli holatga o'tishni boshlash uchun ma'lum tayanch o'zgarishlariga ta'sir qiladi.
   * **shouldComponentUpdate** - isrof qilingan renderlardan xavotirda bo'lsangiz shouldComponentUpdate unumdorlikni oshirish uchun ajoyib joy, chunki u komponent yangi propsni olgan taqdirda qayta ishlashning oldini olishga imkon beradi. shouldComponentUpdate har doim mantiqiy qiymatini qaytarishi kerak va bu nima ekanligiga asoslanib, komponent qayta ko'rsatilgan yoki yo'qligini aniqlaydi.
   * **componentWillUpdate (deprecated)** - kamdan-kam ishlatiladi. U shouldComponentUpdate-ga ega bo'lgan komponentda componentWillReceiveProps o'rniga ishlatilishi mumkin (lekin oldingi propslarga kirish imkoni yo'q).
   * **componentDidUpdate** - shuningdek, odatda props yoki state o'zgarishlariga javoban DOMni yangilash uchun ishlatiladi.
   * **componentWillUnmount** - har qanday chiquvchi tarmoq so'rovlarini bekor qilish yoki komponent bilan bog'langan barcha voqea tinglovchilarini o'chirish imkonini beradi.

13. **React-da referatlar nima uchun ishlatiladi?**
    * Reflar DOM tuguniga yoki React-dagi komponentning namunasiga havola olish uchun ishlatiladi. Fokus/matn tanlashni boshqarish, imperativ animatsiyalarni ishga tushirish yoki uchinchi tomon DOM kutubxonalari bilan integratsiya qilish uchun ref'lardan foydalanishning yaxshi misollari. Siz string refs va inline ref callbacks foydalanishdan qochishingiz kerak. Qayta qo'ng'iroq qilish uchun React tomonidan tavsiya etiladi.

14. **Yuqori tartibli komponent nima? (HOC)**
   Yuqori tartibli komponent - bu komponentni qabul qiladigan va yangi komponentni qaytaradigan funksiya. HOC-lar sizga kod, mantiq va bootstrap abstraktsiyasini qayta ishlatishga imkon beradi. Eng keng tarqalgan, ehtimol Redux-ning ulanish funktsiyasi. Oddiy yordam kutubxonalari va oddiy kompozitsiyani almashishdan tashqari, HOClar React Components o'rtasida xatti-harakatlarni almashishning eng yaxshi usuli hisoblanadi. Agar siz bir xil ishni bajaradigan turli joylarda juda ko'p kod yozayotganingizni sezsangiz, ushbu kodni qayta foydalanish mumkin bo'lgan HOCga qayta tiklashingiz mumkin.

15. **arrow function funksiyalaridan foydalanishning qanday afzalliklari bor?**
   * Qo'llanish sohasi xavfsizligi: O'q funktsiyalari ishlamaguncha, har bir yangi funktsiya o'zining ushbu qiymatini aniqladi (konstruktor holatida yangi ob'ekt, qat'iy rejimda funksiya chaqiruvlarida aniqlanmagan, agar funktsiya "ob'ekt usuli" deb ataladigan bo'lsa, asosiy ob'ekt va hokazo). O'q funksiyasi o'zining buni yaratmaydi, qo'shuvchi bajarish kontekstining bu qiymati ishlatiladi.
   * Kompaktlik: strelka funktsiyalarini o'qish va yozish osonroq.
   * Aniqlik: Deyarli hamma narsa o'q funktsiyasi bo'lsa, har qanday muntazam funktsiya qamrovni aniqlash uchun darhol ajralib turadi. Ishlab chiquvchi har doim Ob'ekt nima ekanligini ko'rish uchun keyingi yuqori funktsiya bayonotini qidirishi mumkin.

16. **Sinf komponentini re-renderdan qanday oldini olasiz?**
   * Komponentni render methodidan null qiymatini qaytarish hech narsa displayga chiqmasligini anglatadi, lekin bu komponentning hayot aylanish usullarini ishga tushirishga ta'sir qilmaydi.
   * Agar komponentni ko'p marta qayta re-render muammosi bo'lsa, ikkita variant mavjud. 
      - shouldComponentUpdate hayot aylanish usuli kancasida tekshirishni qo'lda amalga oshirish.  
      - React.Component o‘rniga React.PureComponent dan foydalanish React.PureComponent moslamalari shouldComponentUpdate() ni sayoz props va state bilan taqqoslash. Bu sizga komponentni bir xil props va state bilan qayta ko'rsatishdan qochish imkonini beradi.

17. **React.createElement yordamida quyidagiga nima teng?**
  ```const element = <h1 className="greeting">Hello, world!</h1>;```

  <pre>
  const element = React.createElement(
   "h1",
   { className: "greeting" },
   "Hello, world!"
  );
  </pre>

18. **Redux nima?**
   * Reduxning asosiy g'oyasi shundan iboratki, butun dastur holati bitta do'konda saqlanadi. Do'kon oddiygina javascript ob'ektidir.
   * Holatni o'zgartirishning yagona yo'li - ilovangizdan amallarni yuborish va keyin holatni o'zgartiruvchi ushbu harakatlar uchun reduktorlarni yozish.
   * Butun holatga o'tish reduktorlar ichida saqlanadi va hech qanday nojo'ya ta'sirga ega bo'lmasligi kerak.

19. **Reduxdagi store nima?**
   - Store dastur holatini saqlaydigan JavaScript ob'ektidir. Shu bilan bir qatorda u quyidagi majburiyatlarga ham ega:

   * GetState(); orqali holatga kirishga ruxsat beradi.
   * dispatch(action) orqali yangilash imkonini beradi.
   * subscribe(listener) orqali tinglovchilarni ro'yxatga oladi.
   * subscribe(listener) tomonidan qaytarilgan funksiya orqali tinglovchilarni ro'yxatdan o'chirishni boshqaradi.

20. **Action va reducer o'rtasidagi farq.**
   * Amallar oddiy JavaScript obyektlaridir.
   * Ular bajarilayotgan harakat turini ko'rsatuvchi turga ega bo'lishi kerak.
   * Aslini olganda, harakatlar sizning ilovangizdan do'koningizga ma'lumotlarni yuboradigan foydali ma'lumotlardir.

   Reduktor oddiygina sof funktsiya bo'lib, oldingi holat va harakatni oladi va keyingi holatni qaytaradi.

21. **Redux Thunk nima uchun ishlatiladi?**
   * Redux thunk - bu action o'rniga bir funktsiyani qaytaradigan action yaratuvchilarini yozish imkonini beruvchi vositachi dastur(middleware).
   * Agar ma'lum bir shart bajarilgan bo'lsa, thunk keyin actionni dispatchini kechiktirish uchun ishlatilishi mumkin. Bu sizga actionlarning asinxron jo'natishni boshqarish imkonini beradi.

22. **React-da propslarni qanday tekshirish mumkin?**
   - Biz "prop-types" paketidan foydalanishimiz mumkin
   - Ilgari, React v15.5 ga qadar bu React iteslfning bir qismi sifatida mavjud edi

<pre>
   import PropTypes from "prop-types";

   function MyComponent({ name }) {
     return <div>Hello, {name}</div>;
   }

   MyComponent.propTypes = {
     name: PropTypes.string,
   };

   export default MyComponent;
</pre>

23. **React HOCga amaliy misol keltiring.**
   Komponent ma'lumotni kutayotganda loaderni ko'rsatish:

<pre>
   //HOC
   function WithLoading(Component) {
     return function WihLoadingComponent({ isLoading, ...props }) {
       if (!isLoading) return <Component {...props} />;
       return <p>Please wait, fetching your data in no time...</p>;
     };
   }
   export default WithLoading;

   //usage
   import UserListComponent from "./UserListComponent.js"; //importing component
   import WithLoading from "./withLoading.js"; //importing HOC
   const ListWithLoading = WithLoading(UserListComponent); //connect component with HOC

   const App = () => {
     const [loading, setLoading] = useState(true);
     const [users, setUsers] = useState([]);
     useEffect(() => {
       //fetch data
       const dataFromApi = ["this is coming from API call", "don't show loader"];
       //at this time loader will be shown in the UI using HOC
       //data fetched successfully
       setUsers([...dataFromApi]);
       setLoading(false);
     }, []);

     return <ListWithLoading isLoading={loading} users={users} />;
   };
</pre>

24. **Reactning useDeferredValue kancasi nima uchun foydali?**
   * "useDeferredValue" - bu foydalanuvchi interfeysining bir qismini yangilashni kechiktirish imkonini beruvchi React Hook.
   * Asosan, bu sizga kamroq kod bilan debouncing texnikasini bajarishga imkon beradi.

25. **Npx va npm o'rtasidagi farq nima?**
   * NPM paketlar menejeri va node.js paketlarini o'rnatish uchun ishlatilishi mumkin.
   * NPX node.js paketlarini execute(bajarish) qilish uchun vositadir.

26. Best Pracise setnumberni ichda callbackdan foydalanish:
    <pre>
     onClick={() => {
          setNumber(number + 1);
     }} ❌
    </pre>
    <pre>
     onClick={() => {
          setNumber((n) => n + 1);
     }} ✅
    </pre>

27. **UseMemo va useCallback o'rtasidagi farq nima?**
   * useCallback sizga funksiyalar uchun renderlar oʻrtasida mos yozuvlar tengligini beradi. UseMemo esa qiymatlar uchun renderlar oʻrtasida mos yozuvlar tengligini beradi.
   * useCallback va useMemo ikkala ham funktsiyani va dependecsyda arrayni kutadi. Farqi shundaki, useMemo o'z funksiyasini chaqirib, natijani qaytarganda, dependencylar o'zgarganda useCallback funksiyani qaytaradi.
   * useCallback o'z funksiyasini chaqirilmagan holda qaytaradi, shuning uchun uni keyinroq qo'ng'iroq qilishingiz mumkin, useMemo esa o'z funksiyasini chaqiradi va natijani qaytaradi.

28. **UseEffect kancasi nima uchun ishlatiladi?**
   * UseEffect kancasi funktsional komponentlarda nojo'ya ta'sirlarni amalga oshirish uchun ishlatiladi. Bu maʼlumotlarni olish, obunalarni sozlash yoki DOMni qoʻlda oʻzgartirish kabi narsalarni oʻz ichiga olishi mumkin. UseEffect kancasi komponent ko'rsatilgandan so'ng chaqiriladi va komponentingiz har qanday tegishli ma'lumotlar yoki bog'liqliklar bilan yangilanib turishini ta'minlash uchun ishlatilishi mumkin.

29. **Vanilla javascript loyihangiz uchun custom useState hookni yarating.**
   <pre>
   function useState(initialState) {
      let state = initialState;
      function setState(newState) {
        //we can also add few conditions to validate the data.
        state = newState;
        render(); //your custom method to trigger page refresh on state change
      }
      return [state, setState];
   } 
   </pre>

30. **PureComponent** Oddiy Componentga o'xshaydi, lekin u bir xil props va state uchun re-renderni o'tkazib yuboradi. Sinf komponentlari hali ham React tomonidan qo'llab-quvvatlanadi, ammo biz ularni yangi kodda ishlatishni tavsiya etmaymiz.

31. **Shadow DOM va Virtual DOM farqi?**
  * Shadow DOM brauzer texnologiyasi bo'lib, asosan veb-komponentlardagi o'zgaruvchilar va CSS-ni aniqlash uchun mo'ljallangan. Virtual DOM - bu JavaScript-dagi kutubxonalar tomonidan brauzer API-lari ustida amalga oshirilgan kontseptsiya.

 
32. **16.3+ versiyadan oldin:**
    <img src='https://github.com/sudheerj/reactjs-interview-questions/blob/master/images/phases16.4.png' alt=''/>

33. **16.3 versiyadan oldin:**
    <img src='https://github.com/sudheerj/reactjs-interview-questions/raw/master/images/phases.png' alt='' /> 

34. **Portal** - bu asosiy komponentning DOM ierarxiyasidan tashqarida mavjud bo'lgan DOM tuguniga bolalarni ko'rsatishning tavsiya etilgan usuli.
    
   <pre>ReactDOM.createPortal(child, container)</pre>

35. **React v16 da Error Boundary qanday?**
   Error Boundary - JavaScript xatolarini bolalar komponentlar daraxtining istalgan joyida ushlaydigan, bu xatolarni qayd etadigan va buzilgan komponentlar daraxti o'rniga zaxira foydalanuvchi interfeysini ko'rsatadigan komponentlar.

36. **Key sifatida indexni berishning tasiri.** 
   Agar siz noyob kalit uchun element ma'lumotlaridan foydalansangiz, todo.id ushbu ro'yxatga xos va barqaror deb hisoblasangiz, React elementlarni qayta ko'rib chiqishga hojat qoldirmasdan qayta tartiblashi mumkin bo'ladi.

37. **Komponentni setStateni chaqirmasdan re-render qilishda majbur qila olasizmi?**
   Odatiy bo'lib, komponentingiz state yoki props o'zgarganda, komponentingiz re-render buladi. Agar render() method boshqa maʼlumotlarga bogʻliq boʻlsa, forceUpdate()ni chaqirib, Reactga komponentni re-ender kerakligini aytishingiz mumkin.
   
   ```component.forceUpdate(callback);```

38. **Redux-saga va redux-thunk o'rtasidagi farqlar qanday?**
   Redux Thunk ham, Redux Saga ham nojo'ya ta'sirlarni bartaraf etishda g'amxo'rlik qiladi. Ko'pgina stsenariylarda Thunk ular bilan shug'ullanish uchun va'dalardan foydalanadi, Saga esa Generatorlardan foydalanadi. Thunk-dan foydalanish oson va Promises ko'plab ishlab chiquvchilarga tanish, Sagas/Generatorlar kuchliroq, ammo siz ularni o'rganishingiz kerak bo'ladi. Ammo ikkala o'rta dastur birgalikda mavjud bo'lishi mumkin, shuning uchun siz Thunks bilan boshlashingiz va kerak bo'lganda/agar kerak bo'lsa, Sagas bilan tanishishingiz mumkin.