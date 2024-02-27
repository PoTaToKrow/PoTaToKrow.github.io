<!--<button class="buttonnn" id="1" >показать</button>-->



<script>


const name_artist_group = "KIBOKO > BEST EVER";
const city = "Санкт-Петербург";
const name_contact = "Лучик Света";
const url_contactor_vk = "https://vk.com/nas.anastasia";
const phone_contactor = "89777777777";
const email_contactor = "morofin1@mail.ru";
const url_group_vk = "https://vk.com/trimetralda";
const url_video = "https://youtu.be/j2YzPg9deJM?si=dx7MdRFepQ2BaATZ";
const url_audio = "https://yandex.music.ru/kiboko";
const webhook = "https://b24-w9syd8.bitrix24.ru/rest/1/tn54l4gvsjfrc534/";

const params = {
  fields: {
    TITLE: name_artist_group,
    STAGE_ID: 'NF1',
    OPENED: 'Y',
    NAME: name_contact,
    PHONE: [{ "VALUE": phone_contactor, "VALUE_TYPE": "WORK" }],
    EMAIL: [{ "VALUE": email_contactor, "VALUE_TYPE": "WORK" }],
    COMMENTS: `Название артиста/группы > ${name_artist_group}\nГород > ${city}\nКонтактное лицо > ${name_contact}\nСсылка на страничку вк > ${url_contactor_vk}\nТелефон > ${phone_contactor}\nE-mail > ${email_contactor}\nСсылка на группу вк > ${url_group_vk}\nСсылка на видео > ${url_video}\nСсылка на аудио > ${url_audio}`
  }
};


const url = "https://b24-w9syd8.bitrix24.ru/rest/1/tn54l4gvsjfrc534/crm.lead.add";

    function sendPost() {
        var httpRequest = new XMLHttpRequest()
        httpRequest.onreadystatechange = function (data) {
            // code
        }
        httpRequest.open('POST', url)
        httpRequest.setRequestHeader('Content-type','application/json')
        httpRequest.send(JSON.stringify(params))
        httpRequest.onload = function() {
          if (httpRequest.status != 200) { // анализируем HTTP-статус ответа, если статус не 200, то произошла ошибка
            alert(`Ошибка ${httpRequest.status}: ${httpRequest.statusText}`); // Например, 404: Not Found
          } else { // если всё прошло гладко, выводим результат
            alert(`Готово, получили ${httpRequest.response.length} байт`); // response -- это ответ сервера
          }
        };
    }
    
 flag = 0;
    var element = document.getElementsByClassName('t-form__submit')[0];
    if (flag == 0) {
        element.addEventListener("submit", event => {
        sendPost()});
        flag++
    }
 
 //const formElement = document.getElementsByClassName('t-form js-form-proccess t-form_inputs-total_9'); // извлекаем элемент формы
 //formElement.addEventListener('submit', (e) => {
  //e.preventDefault();
  //const formData = new FormData(formElement); // создаём объект FormData, передаём в него элемент формы
   //теперь можно извлечь данные
  //const name = formData.get('name_artist_group'); // 'John'
  //const city = formData.get('city'); // 'Smith'
  //alert(`Готово ${name} байт`);
//});
    
    
</script>