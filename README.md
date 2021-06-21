# Gameplay
App develope during NLW Together

## Notes
- We need to define the import type for `.png` files
  - Create a `@types` folder, inside `src` folder, and add a file `png.d.ts`
    ```ts
    declare module "*.png"
    ``` 
- Use brekline to spread your text in multiple lines.
  ```ts
  <Text style={styles.title}>
    Conecte-se {`\n`}
    e organize suas {`\n`}
    jogatinas
  </Text>
  ```
- Organize your styles. Create a file `src/global/styles/theme.ts`
  ```ts
  export const theme = {
    color: {
      background: '#0D133D'
    }
  }
  ```
- Set a resize mode
  ```ts
  <Image  source={IllustrationImg} 
          style={styles.image}
          resizeMode="stretch" />
  ```
- Personalize status bar
  ```ts
  <StatusBar barStyle="light-content" backgroundColor="transparent" translucent />
  ```