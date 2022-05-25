# react_practice
--------REACT-----------

1)react createElement:
 uses an object to assign properties 
    {
        children: ["hello","world"],
        className: "container"
    }
    children can be string, array of string or another HTML element like React.createElement('span',null,"hello","world") ...another way to assign children.

2)JSX
    It is HTML like syntax in JS. But browser uses babel JS compiler to understand it.
    const element=<div className="container">Hello world</div>--->syntax of JSX in script tag