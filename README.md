# SOCIAL OPLESK
### 💼 KIT 
<br/>

## ⚡️ Kit React Form⚡️
<br/> 

## 🏆 K-1 (SimpleForm)

Form 1
```
import React, { useState } from 'react';
import 'bulma/css/bulma.css';



const SimpleForm = () => {
  const [inputValue, setInputValue] = useState('');

  const handleSend = () => {
    const data = { value: inputValue };
    console.log(JSON.stringify(data));
  };

  const handleClear = () => {
    setInputValue('');
  };

  return (
    <div className="container" style={{ maxWidth: 400, marginTop: 40 }}>
      <div className="field">
        <label className="label">Ingresa un valor</label>
        <div className="control">
          <input
            className="input"
            type="text"
            placeholder="Escribe algo..."
            value={inputValue}
            onChange={e => setInputValue(e.target.value)}
          />
        </div>
      </div>
      <div className="buttons">
        <button className="button is-primary" onClick={handleSend}>
          Enviar JSON
        </button>
        <button className="button is-danger" onClick={handleClear}>
          Borrar
        </button>
      </div>
    </div>
  );
};

export default SimpleForm;
```

## 🏆 K-2 (Form)

Form 2
```
import React, { useState } from 'react';
import 'bulma/css/bulma.css';

const MediumForm = () => {
  const [input1, setInput1] = useState('');
  const [input2, setInput2] = useState('');
  const [selectValue, setSelectValue] = useState('');

  const handleSend = () => {
    const data = {
      input1,
      input2,
      selectValue,
    };
    console.log(JSON.stringify(data));
  };

  const handleClear = () => {
    setInput1('');
    setInput2('');
    setSelectValue('');
  };

  return (
    <div className="container" style={{ maxWidth: 400, marginTop: 40 }}>
      <div className="field">
        <label className="label">Primer valor</label>
        <div className="control">
          <input
            className="input"
            type="text"
            placeholder="Escribe el primer valor..."
            value={input1}
            onChange={e => setInput1(e.target.value)}
          />
        </div>
      </div>

      <div className="field">
        <label className="label">Segundo valor</label>
        <div className="control">
          <input
            className="input"
            type="text"
            placeholder="Escribe el segundo valor..."
            value={input2}
            onChange={e => setInput2(e.target.value)}
          />
        </div>
      </div>

      <div className="field">
        <label className="label">Selecciona una opción</label>
        <div className="control">
          <div className="select is-fullwidth">
            <select
              value={selectValue}
              onChange={e => setSelectValue(e.target.value)}
            >
              <option value="">Elige una opción</option>
              <option value="opcion1">Opción 1</option>
              <option value="opcion2">Opción 2</option>
              <option value="opcion3">Opción 3</option>
            </select>
          </div>
        </div>
      </div>

      <div className="buttons">
        <button className="button is-primary" onClick={handleSend}>
          Enviar JSON
        </button>
        <button className="button is-danger" onClick={handleClear}>
          Borrar
        </button>
      </div>
    </div>
  );
};

export default MediumForm;
```


## 🏆 K-3 (Form)

Form 3
```
import React, { useState } from 'react';
import 'bulma/css/bulma.css';

const SimpleForm = () => {
  const [inputValue, setInputValue] = useState('');
  const [radioValue, setRadioValue] = useState('');
  const [check1, setCheck1] = useState(false);
  const [check2, setCheck2] = useState(false);

  const handleSend = () => {
    const data = {
      inputValue,
      radioValue,
      check1,
      check2,
    };
    console.log(JSON.stringify(data));
  };

  const handleClear = () => {
    setInputValue('');
    setRadioValue('');
    setCheck1(false);
    setCheck2(false);
  };

  return (
    <div className="container" style={{ maxWidth: 400, marginTop: 40 }}>
      {/* Input de texto */}
      <div className="field">
        <label className="label">Valor</label>
        <div className="control">
          <input
            className="input"
            type="text"
            placeholder="Escribe algo..."
            value={inputValue}
            onChange={e => setInputValue(e.target.value)}
          />
        </div>
      </div>

      {/* Radios */}
      <div className="field">
        <label className="label">Selecciona una opción</label>
        <div className="control">
          <label className="radio">
            <input
              type="radio"
              name="radioGroup"
              value="opcionA"
              checked={radioValue === 'opcionA'}
              onChange={() => setRadioValue('opcionA')}
            />
            &nbsp;Opción A
          </label>
          &nbsp;&nbsp;
          <label className="radio">
            <input
              type="radio"
              name="radioGroup"
              value="opcionB"
              checked={radioValue === 'opcionB'}
              onChange={() => setRadioValue('opcionB')}
            />
            &nbsp;Opción B
          </label>
        </div>
      </div>

      {/* Checklists */}
      <div className="field">
        <label className="label">Selecciona los checks</label>
        <div className="control">
          <label className="checkbox">
            <input
              type="checkbox"
              checked={check1}
              onChange={() => setCheck1(!check1)}
            />
            &nbsp;Check 1
          </label>
        </div>
        <div className="control">
          <label className="checkbox">
            <input
              type="checkbox"
              checked={check2}
              onChange={() => setCheck2(!check2)}
            />
            &nbsp;Check 2
          </label>
        </div>
      </div>

      {/* Botones */}
      <div className="buttons">
        <button className="button is-primary" onClick={handleSend}>
          Enviar JSON
        </button>
        <button className="button is-danger" onClick={handleClear}>
          Borrar
        </button>
      </div>
    </div>
  );
};

export default SimpleForm;

```


---
<h3 align="center">SOCIAL OPLESK</h3>
