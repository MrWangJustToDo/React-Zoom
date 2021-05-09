## 一个 React 组件,帮助进行图片放大显示

### use

```
import Zoom from 'zoom';

const Test = () => {
  const [i, setI] = useState(1);
  console.log(i);

  return (
    <div>
      <button onClick={() => setI((i) => i + 1)}>按钮</button>
      <Zoom>
        {i % 2 === 0 ? (
          <img className="foo" src="../../6_Animation/Image/image2.jpg" />
        ) : (
          <span>123</span>
        )}
      </Zoom>
    </div>
  );
};

ReactDOM.render(<Test />, document.querySelector("#container"));
```
