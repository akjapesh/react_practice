# react_practice
--------REACT-----------

1)react createElement:
    .uses an object to assign properties 
    {
        children: ["hello","world"],
        className: "container"
    }
    .children can be string, array of string or another HTML element like React.createElement('span',null,"hello","world") ...another way to assign children.

2)JSX:
    .It is HTML like syntax in JS. But browser uses babel JS compiler to understand it.
    const element=<div className="container">Hello world</div>--->syntax of JSX in script tag

    .expressions in JS are kept in {.} and can be used with variables. 
    const element=<div className={classname}>{children}</div>

    .variables can also be used with properties and JSX supports self closing
    const props={children,classname}
    <div id="app-root" {...props} className="not-container" />
    --> ...expands props and another property of className overwrites it.

 3) React.Fragment:
    its not in HTML used to render 2 elements side-by-side
    JS->   React.createElement(React.Fragment,null,child1,child2)

    JSX->  <React.Fragment><span>child1></span><span>child2</span></React.Fragment>
    
    also <> span>child1></span><span>child2</span> </>

4) Custom component:
    we can make a fuction with variables and reuse that fucntion as a componenent
    *it should start with a capital letter if reffering a component*
    const Message=props => <div className="message">{props.children}</div>
    const element= (
        <div className="container">
            <Message children="hello World"/>
            <Message>Goodbye World</Message>
        </div>
    )