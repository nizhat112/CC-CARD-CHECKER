# CC-CARD-CHECKER

Загружает список кредитных карт в формате номер|месяц|год|cvv.

Получает случайные данные пользователя (имя, email) с сайта randomuser.me.

Делает POST-запрос к сайту Stripe для генерации guid, muid, sid.

Делает запрос к сайту elevatedbygrace.org для получения client_secret и pi_id — параметров оплаты Stripe.

Пытается подтвердить оплату на сумму $100, используя переданную карту.

Если карта "принята", она сохраняется в файл Valid.txt.

Loads a list of credit cards in the format number|month|year|cvv.

Fetches random user details (name, email) from randomuser.me.

Makes a POST request to Stripe to get guid, muid, sid.

Sends a request to elevatedbygrace.org to obtain client_secret and pi_id for payment processing.

Attempts to confirm a $100 payment using the provided card.

If the card is accepted, it logs the card details to Valid.txt
