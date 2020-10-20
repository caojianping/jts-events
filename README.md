# jts-events
JavaScript Events的TypeScript封装，提供事件的添加、移除等操作。

## 安装
Using npm:
```bash
$ npm install jts-events
```

Using yarn:
```bash
$ yarn add jts-events
```

## 示例
```ts
import Events from 'jts-events';

// test for events
function testHandler(event: any){
    console.log('bala bala bala!');
}

Events.addEvent(document, 'click', testHandler);
Events.removeEvent(document, 'click', testHandler);
```

## API
##### Events.addEvent(element: any, type: string, handler: Function, userCapture: boolean = false): void
##### Events.removeEvent(element: any, type: string, handler: Function, userCapture: boolean = false): void