import streamlit as st

# MBTI 유형별 특성 설명
mbti_personality_descriptions = {
    'ISTJ': '신뢰할 수 있고, 책임감이 강한 성격을 가지고 있어요. 📚🔍',
    'ISFJ': '다른 사람들을 돕는 것을 좋아하며, 신중하고 조용한 성격이에요. 🏡💖',
    'INFJ': '이해심이 깊고, 이상주의적인 성격을 가지고 있어요. 🕊️✨',
    'INTJ': '차분하고 독립적이며 목표 지향적인 성격을 가지고 있어요. 💡🚀',
    'ISTP': '탐험하고 실험하는 것을 좋아하는 성격이에요. 🔧🧭',
    'ISFP': '예술적이고, 감정적으로 매우 깊은 성격을 가지고 있어요. 🌸🎨',
    'INFP': '상상력이 풍부하고 감정적으로 깊은 성격을 가지고 있어요. 🌌✨',
    'INTP': '논리적이며, 분석적인 성격을 가지고 있어요. 🧠💭',
    'ESTP': '사람들과의 교류를 즐기며, 즉흥적인 성격이에요. 🎉🔥',
    'ESFP': '활발하고 외향적인 성격을 가지고 있어요. 🍉🎈',
    'ENFP': '사람들과의 관계를 중요시하는 개방적인 성격이에요. 💖🌈',
    'ENTP': '창의적이고, 아이디어가 넘치는 성격이에요. 🚀💡',
    'ESTJ': '조직적이고, 실용성을 중시하는 강한 성격이에요. 📋🏢',
    'ESFJ': '사람들과의 교류를 중요시하는 따뜻한 성격이에요. ❤️🎉',
    'ENFJ': '타인의 감정을 잘 이해하며, 리더십을 발휘하는 성격이에요. 🌟👥',
    'ENTJ': '자신감이 넘치고 리더십을 발휘하는 성격이에요. 📈🔥',
}

# MBTI 유형별 궁합 추천
mbti_compatibility = {
    'ISTJ': ('ISFJ', 'ENFP'),
    'ISFJ': ('ISTJ', 'ENTP'),
    'INFJ': ('ENFJ', 'ESTP'),
    'INTJ': ('ENFP', 'ESFJ'),
    'ISTP': ('ESFJ', 'INFJ'),
    'ISFP': ('ENFJ', 'ESTP'),
    'INFP': ('ENFJ', 'ESTJ'),
    'INTP': ('ENTJ', 'ISFJ'),
    'ESTP': ('ISFP', 'INFJ'),
    'ESFP': ('INTJ', 'ISFJ'),
    'ENFP': ('ISTJ', 'INTJ'),
    'ENTP': ('ISFJ', 'INTJ'),
    'ESTJ': ('ISFJ', 'INFP'),
    'ESFJ': ('ISTP', 'INFJ'),
    'ENFJ': ('INFP', 'INTJ'),
    'ENTJ': ('INFP', 'ISFP'),
}

# 제목 설정
st.title('나의 MBTI 특성 분석기 🧠✨')

# MBTI 입력 받기
mbti_type = st.text_input('당신의 MBTI를 입력해주세요! (예: INTJ)')

# 버튼 클릭 시 특성 분석 수행
if st.button('특성 분석하기! 📊'):
    description = mbti_personality_descriptions.get(mbti_type, '올바른 MBTI 유형을 입력해주세요! 🧐')
    if description != '올바른 MBTI 유형을 입력해주세요! 🧐':
        st.write(f'{mbti_type} 님의 특성: {description}')
        best_match, worst_match = mbti_compatibility.get(mbti_type, (None, None))
        st.write(f'가장 잘 맞는 유형: {best_match} 💖')
        st.write(f'가장 잘 안 맞는 유형: {worst_match} 💔')
    else:
        st.write(description)
