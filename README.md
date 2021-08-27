Full Stack Development
----------------------------
-----------------------------

![image](https://github.com/sanskritilakhmani/FullStackDevelopment/blob/main/Full_Stack_Images_/Fullstack.png)

Well! We are breathing in a revolutionized world where everything is digitized, and where the Internet is the need of the hour for everyone. Businesses are moving to an online platform to promote their brands and outreach the customer globally. This technology advancement has impacted the whole world and brings the latest amendments every other day in the software programs. That’s why more and more people want to learn Web Development and adept career as a Web Developer as most of the organizations are looking forward to Front-End developer, Back-End developer, PHP Developer, (.)Net developer, Cloud Architect, Devops Engineer and many more. 


The demand for Full-stack Developers is on the rise. And companies are in desperate need of talented professionals who can work with both Front-End and back-End due to which their demand is hiking. According to the research, there is a 20% growth in demand for Full-stack developer compared to the last couple of years.

![image](https://github.com/sanskritilakhmani/FullStackDevelopment/blob/main/Full_Stack_Images_/Full-Stack-Development-Services-1.jpg)

However, Full-stack Developer holds various skills and knowledge of languages like HTML5, CSS, JavaScript, Angular, and React which comes under front-end development. For back-end, they also possess knowledge regarding NodeJs, Express, phyton, Java, PHP, and multiple databases such as MongoDB, SQL, etc. The role of the full-stack developer is to look at every aspect of software development within an organization.

 React Native Life-Cycle Methods Example-1
 ------------------------------------------


shouldComponentUpdate: This method can be used to avoid unwanted re-renders for better performance. So based on the received new props, we can decide whether to update the component or not.


```
export default class Counter extends React.Component {
  constructor() {
    console.log('Constructor called');
    super();

    this.state = {
      counter: 1,
    };
  }

  componentWillMount() {
    console.log('componentWillMount() called');
  }

  componentDidMount() {
    console.log('componentDidMount() called');
    setInterval(this.update, 2000);
  }

  componentWillUpdate() {
    console.log('componentWillUpdate() called');
  }

  componentDidUpdate() {
    console.log('componentDidUpdate() called');
  }

  update = () => {
    this.setState({ counter: this.state.counter + 1 });
  };
  reset = () => {
    this.setState({ counter: 0 });
  };
  render() {
    console.log('Render called');
    return (
      <View style={styles.container}>
        <Text style={{ textAlign: 'center', margin: 10 }}>
          {this.state.counter}
        </Text>
        <TouchableOpacity style={styles.myButton} onPress={this.update}>
          <Text>{this.props.btitle}</Text>
        </TouchableOpacity>
        <TouchableOpacity
          style={[styles.myButton, { backgroundColor: 'red' }]}
          onPress={this.reset}>
          <Text>Reset</Text>
        </TouchableOpacity>
      </View>
    );
  }
}
```
