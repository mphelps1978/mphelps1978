```js
import react, { useState } from 'React'

const myData = {
  personal: {
    name: 'Michael Phelps',
    location: 'Fairfield, IA, USA',
    age: 42,
    school: 'Lambda School',
    occupation: 'Full Stack Web Developer',
    interests: [
      'programming',
      'gaming and eSports',
      'spending time with family'
    ]
  },
  professional: {
    languages: ['JavaScript', 'HTML', 'CSS', 'React', 'Redux', 'NodeJS', 'Express',],
    databases: ['PostgreSQL', 'SQlite'],
    learning: ['Firebase', 'MongoDB', 'Angular', 'Vue'],
    experience: '1yr'
  },
  contact: {
    email: 'mike@phelpsweb.dev',
    linkedin: 'https://www.linkedin.com/in/michael-phelps1978/',
    twitter: 'https://www.twitter.com/psybermind',
    discord: 'PsyberMind#2418'
  }
}

const MyProfile = () => {
  const [myInfo, setMyInfo] = useState(myData)

  return (
    <div>
      <h1>I'm looking for the chance to prove my skills with you!</h1>
      <h2>Contact me today!</h2>
      { myInfo.array.forEach(element => {
        return(
          <div>
            <p>Name: {element.personal.name}</p>
            <p>email: {element.contact.email}</p>
          </div>
        )})}
    </div>
  )
}
```

Inspired by [martonlederer](https://github.com/martonlederer)
