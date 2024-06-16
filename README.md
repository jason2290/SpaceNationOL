複製以下console腳本

    function clickAllButtons() {
      const treasureButtons = document.querySelectorAll('img#treasure-icon');
      treasureButtons.forEach(button => button.click());
    
      const attackButtons = document.querySelectorAll('div.startBtn');
      attackButtons.forEach(button => button.click());
    
      const autoFillReplyButtons = document.querySelectorAll('p.startBtn');
      autoFillReplyButtons.forEach(button => button.click());
    
      const replyButtons = document.querySelectorAll('span.css-1jxf684');
      replyButtons.forEach(button => {
        if (button.innerText === 'Reply') {
          button.click();
        }
      });
    }
    
    setInterval(clickAllButtons, 1000); 
