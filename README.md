# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

# React basic

### Download Node.js version
www.nodejs.org
___

### Open Terminal
MK New Folder Projectname -> react-project
> npx creact-react-app react-work1

_installing Process_

> cd react-work1

### Open VScode
> react-work1> code . 

### Run browser
> react-work1> npm start

![](https://scontent.fbkk5-1.fna.fbcdn.net/v/t1.6435-9/173468389_10217963224701826_4766939551042572161_n.jpg?_nc_cat=109&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeGzwJk3cs5fZxGWQYvwZltBtALC3F9-zbe0AsLcX37Nt-6rPYZFDiGIXjuSCPo13CU&_nc_ohc=8YjXgCNH4AEAX88MO_b&_nc_ht=scontent.fbkk5-1.fna&oh=8af463ae662e870f37fdcef4c5395e55&oe=609DEC7C)

![](https://saasitive.com/blog/django-react-boilerplate-saas/react_start_project.png)
___

# React Clean-up Project 

### Code Edit
![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.6435-9/173160103_10217963190700976_1148859970658115947_n.jpg?_nc_cat=102&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeH46WpTyN_DsumlZY8TQEOjdS_cX215pyV1L9xfbXmnJYaKxWZPvaWmu7ITRHmnALk&_nc_ohc=9P_mSCVxbAYAX9A8lDe&_nc_ht=scontent.fbkk5-6.fna&oh=3288693cb9ce11a6c7081fd3c85bf8c9&oe=609D8B5B)

### `App.js Edit`


    function App() {
      return (
        <div>Hello React</div>
      );
    }
    
    export default App;

index.css Edit
`empty`

index.js Edit
```
import React from 'react';
import ReactDOM from 'react-dom';

import './index.css';
import App from './App';

ReactDOM.render(<App />, document.getElementById('root'));
```
![](https://scontent.fbkk5-8.fna.fbcdn.net/v/t1.6435-9/171778255_10217963057657650_142011540343071600_n.jpg?_nc_cat=106&ccb=1-3&_nc_sid=825194&_nc_eui2=AeFEbx6fEW_XBxiGGMZt8Gp2jjk1cY-xujaOOTVxj7G6NsZO7-jJkUFt_-aVAgnMpnc&_nc_ohc=abJteQzPnAEAX-xz93G&_nc_ht=scontent.fbkk5-8.fna&oh=4561243f62ae194b519f90095fb5fdf9&oe=609E9685)
---
# Create Todo web
### Edit App.js
```
function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <div>
        <h2>Title</h2>
        <div>
          <button>Delete</button>
        </div>
      </div>
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.6435-9/173001431_10217963343704801_2185854063072279716_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeGAv1aXOYwqj0uOlN57ljc0OmjIDxAAc3c6aMgPEABzdz_CZ6QpDf_gec-CdG8Zlnk&_nc_ohc=-yBthbk50mgAX-_BMLd&_nc_ht=scontent.fbkk5-3.fna&oh=50e9098fa265f191d83b18b49d336897&oe=609DFA8B)

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.6435-0/s403x403/172468626_10217963353785053_3973712093711347927_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeGiKh9X7o4ijJFireQGG3jTKaNWJEvUpgkpo1YkS9SmCThYFJsa1yulgoUNHVk7Szo&_nc_ohc=L9qrT9bPVoYAX-cOpKs&_nc_ht=scontent.fbkk5-3.fna&tp=7&oh=7385c9215ddd9c9c3cbf1d890bbde11b&oe=609F4267)

### Copy CSS to index.css
```
* {
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
  margin: 3rem;
  background-color: #dfdfdf;
}

h1, h2 {
  color: #333333;
}

.btn {
  font: inherit;
  padding: 0.5rem 1.5rem;
  cursor: pointer;
  border-radius: 4px;
  background-color: #800040;
  color: white;
  border: 1px solid #800040;
  margin: 0 1rem;
}

.btn:hover {
  background-color: #9c1458;
  border-color: #9c1458;
}

.btn--alt {
  background-color: transparent;
  color: #800040;
}

.btn--alt:hover {
  background-color: #f8dae9;
}

.card {
  background-color: white;
  border-radius: 4px;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.2);
  padding: 1rem;
  width: 20rem;
}

.actions {
  text-align: right;
}

.modal {
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.2);
  border-radius: 6px;
  background-color: white;
  padding: 1rem;
  text-align: center;
  width: 30rem;
  z-index: 10;
  position: fixed;
  top: 20vh;
  left: calc(50% - 15rem);
}

.backdrop {
  position: fixed;
  z-index: 1;
  background-color: rgba(0, 0, 0, 0.75);
  width: 100%;
  height: 100vh;
  top: 0;
  left: 0;
}
```

### Edit Code App.js
```
function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <div className="card">
        <h2>Title</h2>
        <div>
          <button>Delete</button>
        </div>
      </div>
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.6435-9/174251286_10217963407626399_7181525475775774157_n.jpg?_nc_cat=102&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHJoZIoJHkGXT9Qdg5LveNQHRO71MXLXIsdE7vUxctci8QScSU-ynOGsbaQkyonXp8&_nc_ohc=VhQz1WeSynMAX-HoDyi&_nc_ht=scontent.fbkk5-6.fna&oh=a84520f0560d97c4fb744d596bba4407&oe=609D96B6)

Edit App.js
```
function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <div className="card">
        <h2>Title</h2>
        <div className="action">
          <button className="btn">Delete</button>
        </div>
      </div>
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.6435-9/172670607_10217963422026759_6175109488255212857_n.jpg?_nc_cat=101&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeEr8VqICXfrqukn4rm1pprhL5KUQE5--2wvkpRATn77bJA19aQlAWaJswudANpRqb4&_nc_ohc=cwZQ6WOEhikAX8gmWgt&_nc_ht=scontent.fbkk5-6.fna&oh=7f4ce6c89cb6cab8cf3b28ab24155737&oe=60A0A332)
---

# Build Re-USE Components

### Create Todo.js in Components New Folder

![](https://scontent.fbkk5-1.fna.fbcdn.net/v/t1.6435-9/175149360_10217963457987658_7157506797312817821_n.jpg?_nc_cat=109&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHbUJVB1nJmswKGMnxqXCF-WeRmtYi1gH9Z5Ga1iLWAf6ex90X2QDSspE5A34Jp5Aw&_nc_ohc=ZTK2QouGieYAX86VFeY&_nc_ht=scontent.fbkk5-1.fna&oh=d846a82d0bfa89f90785362d6e099180&oe=609FBE8B)

```
function Todo() {
    return (
        <div className="card">
        <h2>Learn React</h2>
        <div className="action">
          <button className="btn">Delete</button>
        </div>
      </div>
    );
}
export default Todo;
```
![](https://scontent.fbkk5-7.fna.fbcdn.net/v/t1.6435-9/173574684_10217963522069260_329173819956750086_n.jpg?_nc_cat=108&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeGKNfI4yMuP6kp7nv4tw3mBGGlnb8J31-IYaWdvwnfX4hNOg54Ki8wiiGCuv4fqExA&_nc_ohc=0gJYkrHtO9IAX8AUKji&_nc_ht=scontent.fbkk5-7.fna&oh=eb1f9860d7a8b33c4fc7d5fb0daed180&oe=60A05F3E)

### Edit App.js
```
import Todo from './components/Todo';

function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <Todo />
      <Todo />
      <Todo />
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-8.fna.fbcdn.net/v/t1.6435-9/174489354_10217963532189513_840836418589774007_n.jpg?_nc_cat=106&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeE7s_F8QwUFLiuxOy_Lgm26D6G9NffCKBcPob0198IoF6NmBPt-IDa_7mIthGUVuO0&_nc_ohc=B2Bb1LrTdW8AX_fY9p9&_nc_ht=scontent.fbkk5-8.fna&oh=c85b28aa6eb3afe69c3c995748841258&oe=609E2961)

![](https://scontent.fbkk5-5.fna.fbcdn.net/v/t1.6435-9/170753872_10217963548109911_4972001412726807095_n.jpg?_nc_cat=104&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeEnhIz6U74k_jZPC_z7qxMZfsEAQX4ypmZ-wQBBfjKmZoZ0kHggFnG2upg2O1Fw9UU&_nc_ohc=-em6ZfPooeIAX_rYwnY&_nc_ht=scontent.fbkk5-5.fna&oh=c08d43747ca61f6d9f27d03a322cd65b&oe=60A09277)

---

# Passing Data With Props & Dynamic Content
Edit App.js 
```
import Todo from './components/Todo';

function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <Todo text='Learn React' />
      <Todo text='Master React' />
      <Todo text='Full React Course' />
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-5.fna.fbcdn.net/v/t1.6435-9/174232481_10217963634472070_1365470215815342496_n.jpg?_nc_cat=100&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHje7uVVWUEJbiBg4OEw74-vZZDPDUF2vu9lkM8NQXa-4bu4yLJewpXMwST6B6xNbY&_nc_ohc=Q5hMOT4iW_QAX93htKa&_nc_ht=scontent.fbkk5-5.fna&oh=986b17d00f57688919760e3361702001&oe=60A0D09B)

Edit Todo.js for Add Props Function
```
function Todo(props) {
    return (
        <div className="card">
        <h2>{ props.text }</h2>
        <div className="action">
          <button className="btn">Delete</button>
        </div>
      </div>
    );
}
export default Todo;
```

![](https://scontent.fbkk5-7.fna.fbcdn.net/v/t1.6435-9/173752182_10217963649472445_4437285346351937545_n.jpg?_nc_cat=108&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFJGCyOzkUGbk7E9UakE8V8VHID7YH9E3BUcgPtgf0TcNSgCegDvoucKlS2Y3iHchg&_nc_ohc=XJUoFJ_hf-IAX_d1gIF&_nc_ht=scontent.fbkk5-7.fna&oh=14868dbd9647880fb12bec6cb2fc74ed&oe=609EBDD1)

![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.6435-9/173275345_10217963654112561_3109528924779110114_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFqLEQPwjViUrgYZ0fQ1d6vHwG7VsdIAl0fAbtWx0gCXQo7cTIX4R1gLB-uvGSJCVQ&_nc_ohc=ZhZrZvqFo14AX86yfPw&_nc_ht=scontent.fbkk5-3.fna&oh=af106b4ebba33684276a66c5c96744f0&oe=609DD7EB)
---

# Handling Events
### Add Event onClick Button in Todo.js
```
function Todo(props) {
  function deleteHandler() {
    console.log('Clicked');
    console.log(props.text);
  }

    return (
        <div className='card'>
        <h2>{ props.text }</h2>
        <div className='action'>
          <button className='btn' onClick={deleteHandler}>Delete</button>
        </div>
      </div>
    );
}
export default Todo;
```
![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.6435-9/174628970_10217968188145909_8166736330616890836_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeGfYzePK27Y2DkDQ83g5RPXzHbDtm_8WfrMdsO2b_xZ-tHteowr4c0xzZglSLjJyZg&_nc_ohc=fJHbQOYmqfcAX-zsRZf&_nc_ht=scontent.fbkk5-3.fna&oh=2033350badf7a843b44640a3aaa4882d&oe=60A1B9E0)

### Event Click Delete Button
![](https://scontent.fbkk5-7.fna.fbcdn.net/v/t1.6435-9/172350914_10217968199346189_2277179573418907642_n.jpg?_nc_cat=107&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHny53HfcOrPuajHYe_RUnHYD7LKtwGpfVgPssq3Aal9a0lFUZb34mwvQnU2uNKTVM&_nc_ohc=MM207J7EsKQAX9SrUn4&_nc_ht=scontent.fbkk5-7.fna&oh=3e8bcb67e317cc30738cb56a86479bc0&oe=609EE296)
---

# Adding More Overlay Components
### Add New File Modal.js at components Folder
![](https://scontent.fbkk5-6.fna.fbcdn.net/v/t1.6435-9/172580450_10217968297668647_708906136395153756_n.jpg?_nc_cat=102&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeH3ONHP-_h6uLxljYZVhnKB-SZcNmaml-_5Jlw2ZqaX7916HfFcpylr0t6fewyheCw&_nc_ohc=QaG43ityWmwAX-vityD&_nc_ht=scontent.fbkk5-6.fna&oh=a58037b5c3b4dd73e4f98d143532df97&oe=60A24EEE)
```
function Modal() {
    return (
        <div className="modal">
            <p>Are You Sure !</p>
            <button className='btn btn--alt'>Cancel</button>
            <button className='btn'>Confirm</button>
        </div>
    ); 
}

export default Modal;
```
![](https://scontent.fbkk5-5.fna.fbcdn.net/v/t1.6435-9/171916106_10217968456272612_3350330002283868717_n.jpg?_nc_cat=100&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFsZVG_pmu5KDJa9J1yiBkoRG8aDSseAKpEbxoNKx4AqiASaW5kzqPBXE54OKuTIm4&_nc_ohc=CbmV0tC3cxIAX-lHMIQ&_nc_ht=scontent.fbkk5-5.fna&oh=5baf6674dc1c78bab509d1f4cda35839&oe=60A22425)

### Add New File Backdrop.js at components Folder for Background
![](https://scontent.fbkk5-3.fna.fbcdn.net/v/t1.6435-9/175127004_10217968360190210_1401133837248141202_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFIaQnz8tDJHcby0Vo9ja-Bja72FrzYuZaNrvYWvNi5ltSYPO24kTpPSbKHWJ4GWJ8&_nc_ohc=wGIIEmZXSf0AX8THxom&_nc_ht=scontent.fbkk5-3.fna&oh=700254319fd553314877b515f9e17bfb&oe=609ECBAD)

```
function Backdrop() {
    return <div className='backdrop'></div>;
}

export default Backdrop;
```
![](https://scontent.fbkk5-8.fna.fbcdn.net/v/t1.6435-9/171924127_10217968383750799_883805246500915814_n.jpg?_nc_cat=106&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFXxnN_-dRgdV04CSXUhHZqW1TDSep7x2lbVMNJ6nvHacu9LvxHsHs4IqVXMAMwQOE&_nc_ohc=BFCq_a68e2kAX-NdCET&_nc_ht=scontent.fbkk5-8.fna&oh=2495a5d6320f4554260b9b52bae8fd6a&oe=609EB008)

![](https://scontent.fbkk5-7.fna.fbcdn.net/v/t1.6435-9/174604978_10217968464192810_5034445974849273722_n.jpg?_nc_cat=108&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHeJtppRneELoBzeoWN5XM_36sksum6L4zfqySy6bovjFgw6h3FtMVjW2jZ3zz3uzk&_nc_ohc=uDVHDOuV-DwAX-JHIk0&_nc_ht=scontent.fbkk5-7.fna&oh=3ce64388ed79eb74ee59ca6a64a0fa0f&oe=60A1B90B)
---

# Introducing State
### Edit App.js 
```
import Todo from './components/Todo';

function App() {
  return (
    <div>
      <h1>My Todos</h1>
      <Todo text='Learn React' />
      <Todo text='Master React' />
      <Todo text='Full React Course' />
    </div>
  );
}

export default App;
```
![](https://scontent.fbkk5-5.fna.fbcdn.net/v/t1.6435-9/173902520_10217968630436966_670527869753044740_n.jpg?_nc_cat=104&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeE-xDR907_9INS5-gGm9hAy5RYfdYKFe-_lFh91goV771v-vww415wCurQG-a_iTKk&_nc_ohc=IUGrkqFCopgAX94mhmY&_nc_ht=scontent.fbkk5-5.fna&oh=e6c5b44d32b98a839bb54c1d0cee00d0&oe=60A28555)

### Edit Todo.js  add React Hook UseState
```
import { useState } from 'react';

import Modal from './Modal';
import Backdrop from './Backdrop';

function Todo(props) {
  const [ modalIsOpen, setModalIsOpen ] = useState(false);

  function deleteHandler() {
    setModalIsOpen(true);
  }

    return (
        <div className='card'>
        <h2>{ props.text }</h2>
        <div className='action'>
          <button className='btn' onClick={deleteHandler}>Delete</button>
        </div>
        {/* { modalIsOpen ? <Modal /> : null } */}
        { modalIsOpen && <Modal /> }
        { modalIsOpen && <Backdrop /> }
      </div>
    );
}
export default Todo;
```
![](https://scontent.fbkk5-4.fna.fbcdn.net/v/t1.6435-9/173697991_10217968635717098_9036485641483243825_n.jpg?_nc_cat=110&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeF5DgBZntLCwFrE6RHqB17eDn6Gq2OimXYOfoarY6KZdkC5W50QNrYJ26xhzya-els&_nc_ohc=tWADBKa9UbMAX_PVYSr&_nc_ht=scontent.fbkk5-4.fna&oh=cfe0f18186e0368da582f0533715d655&oe=60A1D47D)

### When Click Delete Button
![](https://scontent.fbkk5-4.fna.fbcdn.net/v/t1.6435-9/172436323_10217968639277187_4822316520278362251_n.jpg?_nc_cat=110&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeFcBFJ5DRFSTjfEb6NW1THamnWmA0P2ilWadaYDQ_aKVSabexzgpqLjgKKUl-TB-Ag&_nc_ohc=7Z0H3T-Hv_oAX8pljUX&_nc_ht=scontent.fbkk5-4.fna&oh=b8977861e327858835d3175aa9e77b1f&oe=60A077CD)

### Modal and Backdrop will Shown
![](https://scontent.fbkk5-7.fna.fbcdn.net/v/t1.6435-9/172567481_10217968640117208_8253753330972788752_n.jpg?_nc_cat=107&ccb=1-3&_nc_sid=dbeb18&_nc_eui2=AeHKZKrqMr0tq1iDcFZC4vD8rU7V4zoaye6tTtXjOhrJ7lvbDGT0ukN_s1fbI1XeXXM&_nc_ohc=YTWcLRb_cPAAX9cztsx&_nc_ht=scontent.fbkk5-7.fna&oh=3d6c19809bf59611f5bd34c9a87c3d21&oe=60A0C52D)
