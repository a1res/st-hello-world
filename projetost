import json
import requests
import streamlit as st
from streamlit_lottie import st_lottie
from streamlit_option_menu import option_menu
from PIL import Image

st.set_page_config(page_title='Gabriel Aires', layout='wide')

def load_lottiefile(filepath: str):
    with open(filepath, "r") as f:
        return json.load(f)

def load_lottieurl(url: str):
    r = requests.get(url)
    if r.status_code != 200:
        return None
    return r.json()

lottie_coding = load_lottieurl('https://lottie.host/004b4f44-787c-495f-a1e5-2383fde292a0/qdacVhliv4.json')
lottie_question = load_lottieurl('https://lottie.host/861cba28-e59e-4add-8892-7a21e0babb28/AdAOcDx0mG.json')

#Navigation
selected = option_menu(
    menu_title=None,
    options=['Home', 'Trajetória Pessoal', 'Trajetória Profissional', 'Currículo', 'Contato'],
    icons=['house', 'book', 'collection', 'person-circle','envelope-at'],
    default_index=0,
    orientation='horizontal',
 )
if selected == 'Home':
    col1, col2, col3 = st.columns([3, 6, 3])
    with col2:
        st.title('Bem vindo(a) à minha página pessoal!')
        st.write('''
            Esta página foi desenvolvida por Gabriel Aires da Silva para o processo
            seletivo de estagiários da empresa Sensorville (29/08/2023).
            ''')
        st.write('')
        st.write('')
        st.write('')
    col4, col5, col6, col7 = st.columns([1.5, 4.5, 4.5, 1.5])
    with col5:
        st.header('O processo de criação:')
        st.write('')
        st.write('')
        st.write('''
                 O primeiro desafio foi encontrar o ambiente de trabalho que mais me agradasse.
                 Costumeiramente, eu utilizava o OnlineGDB para compilar códigos e acompanhar
                 as aulas de programação da faculdade, mas, neste caso, não era possível utilizá-lo.
                 Depois de muitas pesquisas e testes, acabei adotando o VSCode, que pareceu intuitivo
                 e moderno.
                 ''')
        st.write('')
        st.write('''
                 Depois de encontrar o meu compilador de códigos, precisei buscar a maneira
                 mais fácil de criar uma aplicação web, e o streamlit foi o escolhido. Os motivos
                 para isso se devem pelo fato de que é uma aplicação bem moderna e acessível 
                 para um iniciante nessa área, visto que eu nunca programei um site antes.
                 ''')
        st.write('')
        st.write('''
                 Após escolher o compilador e a aplicação, passei para as pesquisas. Tive um
                 grande auxílio com o google, o próprio site do streamlit e sua comunidade, o
                 youtube e o ChatGPT. Todas essas ferramentas de busca combinadas me levaram a
                 desenvolver o site que você está acessando agora.
                 ''')
        st.write('''
                 O desenvolvimento do site em si levou aproximadamente dois dias, e os estudos
                 para que isso ocorresse levaram outros cinco. No total, fui designado a terminar
                 esta proposta em 7 dias e acredito ter gerenciado bem o meu tempo para que 
                 nenhum imprevisto acontecesse. Ter saído literalmente do zero e em sete dias
                 chegar a este resultado foi uma experiência muito gratificante e positiva 
                 para o meu aprendizado.
                 ''')
        st.write('')
        st.write('')
    with col6:
            st_lottie(lottie_coding, height=500,  width=500,)

    col8, col9, col10, col11 = st.columns([1.5, 4.5, 4.5, 1.5])
    with col10:
        st.header('O que o site contém:')
        st.write('')
        st.write('')
        st.write('''
                 O site contém uma página inicial (Home), onde eu falo sobre como foi criá-lo 
                 e como foi desenvolvê-lo, além das ferramentas utilizadas e das dificuldades
                 enfrentadas.
                 ''')
        st.write('')
        st.write('''
                 A página da Trajetória Pessoal conta minha história e um pouco
                 mais sobre mim, falando sobre educação e formação, e trazendo também
                 informações e habilidades pessoais que dizem à meu respeito.
                 ''')
        st.write('')
        st.write('''
                 A página de Trajetória Profissional traz minhas experiências dentro
                 e fora da faculdade: desde matérias que tive durante os semestres
                 na UTFPR até a minha coleção de certificados e cursos online que 
                 eu participo sempre que tenho a oportunidade, o interesse e o
                 tempo para concluí-los.
                 ''')
        st.write('')
        st.write('''
                 A página do currículo traz o meu CV completo e atualizado, o qual utilizo
                 para aplicar em vagas de emprego que se encaixem no meu perfil.
                 ''')
        st.write('')
        st.write('''
                 A página de contato traz apenas informações que interessam a quem
                 esteja procurando alguma forma de me contatar, assim como um box completamente
                 funcional em que você preenche com seu nome, email, e mensagem a ser enviada a mim.
                 ''')
    with col9:
        st_lottie(lottie_question)

if selected == 'Trajetória Pessoal':
    col1, col2, col3, col4 = st.columns([2, 3, 6, 2])
    with col2:
        st.write('')
        st.write('')
        image = Image.open('foto rosto.jpeg')
        st.image(image, width=370)
    with col3:
        st.title('Gabriel Aires da Silva')

        
        st.subheader(' :male_sign: Sexo: masculino')
        st.subheader(' :man: Estado Civil: solteiro')
        st.subheader(' :date: Data de nascimento: 07/02/2003')
        st.subheader(' :earth_americas: Nacionalidade: brasileiro')
        st.subheader(':male-student: Escolaridade: UTFPR (cursando 4º período)')
        st.subheader(' :speech_balloon: Línguas: português nativo, inglês fluente e espanhol básico')
        st.write('')
        st.write('')
        st.write('')
        st.write('')

    col5, col6, col7 = st.columns([2, 8, 2])
    with col6:
        st.header('Quem sou eu?')

        st.write('''
                     Sou disciplinado, organizado, focado e tranquilo, principalmente
sob pressão ou diante de desafios. Tenho paixão por esportes,
engenharia, automobilismo, amizades e família. Estas foram algumas
das coisas que me ajudaram a moldar a minha visão de mundo.
Tenho facilidade em aprender de forma autônoma, gosto de desafios,
valorizo conexões interpessoais, prezo pela empatia e comunicação,
aprendo com amigos e gosto da cooperação que o trabalho em equipe traz.
Um exemplo disso é o trabalho voluntário que eu faço já tem mais de um ano,
onde ajudo com a organização do ambiente para que o trabalho possa ser eficaz.
Adquiri diversos conhecimentos universitários que dizem respeito à minha área,
tais como programação em diversas linguagens, manuseio de microcontroladores,
placas de circuito impresso, entre outros; Tudo isso me dá sinais
claros de que a engenharia eletrônica me trará a oportunidade de fazer
parte de transformações significativas na área de tecnologia, automação, 
robótica e inovação, que impactam profundamente na sociedade, na
economia e na forma como vivemos. Dessa forma, são desenvolvidas novas
soluções, novos produtos e serviços, todos atendendo necessidades da
humanidade. Estou ansioso para aplicar minhas competências e conhecimentos,
aprender e crescer como membro de uma equipe de estágio, ajudando a
transformar projetos em soluções para os clientes e para o mercado.
                     ''')
        st.markdown('***')
        st.header('Abaixo, listo algumas das minhas habilidades pessoais:')
        col9, col10, col11, col12 = st.columns([1, 4, 4, 1])
        with col10:
            st.write('')
            st.write('')
            st.write('')
            st.subheader(':heavy_check_mark: Escrita')
            st.write('')
            st.subheader(':heavy_check_mark: Disciplina')
            st.write('')
            st.subheader(':heavy_check_mark: Organização')
            st.write('')
            st.subheader(':heavy_check_mark: Comunicação')
            st.write('')
            st.subheader(':heavy_check_mark: Autoaprendizado')
        with col11:
            st.write('')
            st.write('')
            st.write('')
            st.subheader(':heavy_check_mark: Solução de problemas')
            st.write('')
            st.subheader(':heavy_check_mark: Relacionamento interpessoal')
            st.write('')
            st.subheader(':heavy_check_mark: Colaboração virtual')
            st.write('')
            st.subheader(':heavy_check_mark: Fluência digital')
            st.write('')
            st.subheader(':heavy_check_mark: Adaptabilidade e flexibilidade')

if selected == 'Trajetória Profissional':
    
    st.text("")
    col6, col7, col8=st.columns([2.5, 8, 2])
    with col7:
        st.title('Aqui você encontrará algumas das minhas conquistas')
    st.text("")
    st.text("")
    st.text("")
    col1, col2, col3, col4 = st.columns([2, 2, 5, 1])
    with col2:
        st.text(" ")
        st.text(" ")
        image = Image.open('UTFPR.jpg')
        st.image(image, width=300)
        st.text(" ")
        st.text(" ")
        st.text(" ")
        image = Image.open('PowerBi.jpg')
        st.image(image, width=300)
        st.text(" ")
        image = Image.open('Excel.jpg')
        st.image(image, width=180)
        st.text(" ")
        image = Image.open('C.jpg')
        st.image(image, width=150)
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        image = Image.open('PythonLogo.jpg')
        st.image(image, width=300)
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        image = Image.open('Chatgpt.jpg')
        st.image(image, width=300)
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        st.text(" ")
        image = Image.open('INCBAC.jpg')
        st.image(image, width=300)
        st.text(" ")
        st.text(" ")
        image = Image.open('Cambridge.jpg')
        st.image(image, width=200)
        image = Image.open('Canada.jpg')
        st.image(image, width=300)

    with col3:
        #Fonte do header
        st.markdown("""
        <style>
        .header {
        font-size:30px !important;
        }
        </style>
        """, unsafe_allow_html=True)

        #Fonte do subheader
        st.markdown("""
        <style>
        .subheader {
        font-size:25px !important;
        }
        </style>
        """, unsafe_allow_html=True)

        st.markdown('<p class="header">APROVADO NA UNIVERSIDADE TECNOLÓGICA FEDERAL DO PARANÁ</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Atualmente cursando o quarto período de engenharia eletrônica</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">NÍVEL INTERMEDIÁRIO EM POWER BI</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Curso online gratuito e certificado pela Fundação Bradesco</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">NÍVEL INTERMEDIÁRIO EM EXCEL</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Curso online gratuito e certificado pela Fundação Bradesco</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">CONHECIMENTO EM LINGUAGEM C DE PROGRAMAÇÃO</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Matéria estudada na faculdade, com foco em programação de computador e estrutura de dados</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">CONHECIMENTO EM LINGUAGEM PYTHON DE PROGRAMAÇÃO</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Matéria estudada na faculdade como uma introdução à algorítmos</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">CONHECIMENTO EM IA</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Curso online gratuito sobre ChatGPT certificado pela Prime Cursos</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">ARITGO CIENTÍFICO INTERNACIONAL</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Treinamento online pelo Instituto INCBAC para publicação de um artigo científico internacional</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">FIRST ENGLISH CERTIFICATE</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Certificado de Cambridge pela conclusão do teste FCE</p>', unsafe_allow_html=True)
        st.markdown('***')
        st.markdown('<p class="header">EXCHANGE PROGRAM</p>', unsafe_allow_html=True)
        st.markdown('<p class="subheader">Intercâmbio de 3 semanas realizado no Canadá e promovido pelo Colégio Bom Jesus</p>', unsafe_allow_html=True)

if selected == 'Currículo':
    col1, col2, col3 = st.columns(3)
    with col2:
        image = Image.open('Currículojpg.jpg')
        st.image(image, width=700)

if selected == 'Contato':
    st.title('Sinta-se à vontade para me contatar!')
    st.markdown('''
                **-Telefone:** +55 (41) 99986-8097\n
                **-Linkedin:** https://www.linkedin.com/in/gabriel-aires-da-silva/\n
                **-Instagram:** https://www.instagram.com/aires.ds/\n\n
                Ou então, envie um e-mail aqui abaixo para mim, ou
                diretamente em **gab.aires.03@gmail.com**.\n
                ''')
    contact_form = """
    <form action="https://formsubmit.co/gab.aires.03@gmail.com" method="POST">
    <input type="hidden" name="_captcha" value="false">
    <input type="text" name="name" placeholder='Seu nome' required>
    <input type="email" name="email" placeholder='Seu e-mail' required>
    <textarea name='mensagem' placeholder='Sua mensagem'></textarea>
    <button type="submit">Enviar</button>
    </form>
    """
    st.markdown(contact_form, unsafe_allow_html=True)

    def local_css(file_name):
        with open(file_name) as f:
            st.markdown(f'<style>{f.read()}</style>', unsafe_allow_html=True)

    local_css("style.css")
