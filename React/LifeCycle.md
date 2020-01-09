## Life Cycle

컴포넌트를 생성할 때에는 constructor -> componentWillMount -> render -> componentDidMount순서로 진행되며 컴포넌트를 제거할 때에는 componentWillUnmount prop이 변경될 때에는 componentWillReceiveProps -> shouldComponentUpdate -> componentWillUpdate -> render -> componentDidUpdate순으로 진행되는 것으로 알고 있습니다.

constructor : 생성자 메소드로서 컴포넌트가 처음 만들어질 때 실행되는 메소드
componentWillMount : 컴포넌트가 DOM위에 만들어지기 전에 실행되는 메소드
render : 컴포넌트 렌더링을 담당
componentDidMount : 컴포넌트가 만들어지고 첫 렌더링을 다 마친 후 실행되는 메소드
componentWillReceiveProps : 컴포넌트가 props을 새로 받았을 때 실행되는 메소드
shouldComponentUpdate : prop혹은 state가 변경되었을 때 리렌더링 할지 말지 정하는 메소드
componentWillUpdate : 컴포넌트가 업데이트 되기 전에 실행되는 메소드
componentDidUpdate : 컴포넌트가 리렌더링을 마친 후 실행되는 메소드
componentWillUnmount : 컴포넌트가 DOM에서 사라진 후 실행되는 메소드