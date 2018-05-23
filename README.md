# validateForm
        <form id="form1" data-reachgoal="main-form">
            <input
                    name="name"
                    class="Input"
                    data-validator="letters"
            />
            <input
                    type="tel"
                    name="phone"
                    class="Input"
                    placeholder="+7 (___) ___-__-__"
                    data-validator="regexp"
                    data-validator-pattern="^((8|\+7)[\- ]?)?(\(?\d{3}\)?[\- ]?)?[\d\- ]{7,10}$"
            />
            <textarea
                    class="FormSection-Textarea"
                    name="appeal-text"
                    data-validator="empty"
                    data-required
            ></textarea>
            <select class="FormSection-Select"
                    name="break-type"
                    data-validator="empty"
                    data-required
            >
                <option value="">Выберите тип</option>
                <option value="Благодарность">Благодарность</option>
            </select>
            <button class="Btn">
                Получить консультацию
            </button>
        </form>
        
### script init
    validateForm({
        formId: 'form1'
        //formValidClass: 'Form_valid',
        //formInvalidClass: 'Form_invalid',
        //inputErrorClass: 'Input_error'
    });
