### Identidades de Traço no espaço de Minkowski

#### Gerais

Sejam $\alpha,\beta \in \mathbb{C}$.
$$
\begin{align}
    &* \text{tr}\left[ \alpha A + \beta B \right] = \alpha\text{tr}\left[A\right] + \beta\text{tr}\left[B\right] \\
    &* \text{tr}\left[ABC\right] = \text{tr}\left[BCA\right] = \text{tr}\left[CAB\right]
\end{align}
$$

#### Matrizes Gamma de Dirac
$$
\begin{align}
    &* \text{tr}\left[ \gamma_\mu \right] = 0 \\
    &* \text{tr}\left[ \gamma_\mu \gamma_\nu \right] = 4 g_{\mu\nu} \\
    &* \text{tr}\left[ \gamma_\mu \gamma_\nu \gamma_\rho \right] = 0 \\
    &* \text{tr}\left[ \gamma_\mu \gamma_\nu \gamma_\rho \gamma_\lambda \right] = 4\left( g_{\mu\nu}g_{\rho\lambda} - g_{\mu\rho}g_{\nu\lambda} + g_{\mu\lambda}g_{\nu\rho} \right) \\
\end{align}
$$

#### Notação Slash de Feynman

Seja $k\!\!\!/ = k^\mu \gamma_\mu$. \\
$$
\begin{align}
    &* \text{tr}\left[ k\!\!\!/ \right] = k^\mu \text{tr}\left[ \gamma_\mu \right] = 0 \\
    &* \text{tr}\left[ k\!\!\!/ k\!\!\!/ \right] = k^\mu k^\nu \text{tr}\left[ \gamma_\mu \gamma_\nu \right] = 4 k^\mu k^\nu g_{\mu\nu} = 4 k^2 \\
    &* \text{tr}\left[ k\!\!\!/ q\!\!\!/ \right] = k^\mu q^\nu \text{tr}\left[ \gamma_\mu \gamma_\nu \right] = 4 k^\mu q^\nu g_{\mu\nu} = 4(k \cdot q)
\end{align}
$$

### Identidades de Traço no espaço euclidiano

Em Minkowski $(-,+,+,+)$, as matrizes de Dirac satisfazem a relação de anticomutação
$$
\begin{equation}
    \{ \gamma_\mu, \gamma_\nu \} = 2 g_{\mu\nu} \mathbb{I}
\end{equation}
$$

e por isso $\text{tr}\left[ \gamma_\mu \gamma_\nu \right] = 4 g_{\mu\nu}$.

Agora, em espaço euclidiano, satisfazem uma álgebra de Clifford
$$
\begin{equation}
    \{ \gamma_\mu, \gamma_\nu \} = 2 \delta_{\mu\nu} \mathbb{I}
\end{equation}
$$

e, portanto, temos
$$
\begin{equation}
    \mathrm{tr}\left[ \gamma_\mu \gamma_\nu \right] = 4 \delta_{\mu\nu}.
\end{equation}
$$

O mesmo vale para as outras identidades supracitadas: a delta de Kronecker aparece no lugar da métrica.

### Cálculo do traço da _Equação de Gap_ em espaço euclidiano

A equação de Dyson-Schwinger em questão é:
$$
\begin{equation}
    i p\!\!\!/ A(p^2) + B(p^2) - ip\!\!\!/ - m_0 = \bar{g}^2 \int_k \gamma_\mu \frac{-i k\!\!\!/ A(k^2) + B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2} \gamma_\nu
\end{equation}
$$

Primeiramente, multiplicamos a equação por $p\!\!\!/$:
$$
\begin{align*}
    i p\!\!\!/ p\!\!\!/ A(p^2) + p\!\!\!/ B(p^2) - ip\!\!\!/ p\!\!\!/ - p\!\!\!/m_0 &= p\!\!\!/ \bar{g}^2 \int_k \gamma_\mu \frac{-i k\!\!\!/ A(k^2) + B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2} \gamma_\nu
    \\
    &= \bar{g}^2 \int_k \frac{-i p\!\!\!/ \gamma_\mu k\!\!\!/ \gamma_\nu A(k^2) + p\!\!\!/ \gamma_\mu \gamma_\nu B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
    \\
    &= -i\bar{g}^2 \int_k  \frac{p\!\!\!/ \gamma_\mu k\!\!\!/ \gamma_\nu A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
    \\
    &\ \ \ \ + \bar{g}^2 \int_k \frac{p\!\!\!/ \gamma_\mu \gamma_\nu B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
\end{align*}
$$

e então tomamos o traço. O lado esquerdo fica:
$$
\begin{align*}
    i \text{tr}\left[ p\!\!\!/ p\!\!\!/ \right]A(p^2) + \text{tr}\left[ p\!\!\!/ \right] B(p^2) - i\text{tr}\left[ p\!\!\!/ p\!\!\!/ \right] - \text{tr}\left[ p\!\!\!/ \right]m_0 = 4ip^2 A(p^2) - 4ip^2
\end{align*}
$$

e o lado direito fica:
$$
\begin{align*}
    i\bar{g}^2 \int_k  \frac{ \text{tr} \left[p\!\!\!/ \gamma_\mu k\!\!\!/ \gamma_\nu\right] A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} &\left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
    \\
    &= -i\bar{g}^2 \int_k  \frac{ p^\rho k^\sigma \text{tr} \left[\gamma_\rho \gamma_\mu \gamma_\sigma \gamma_\nu\right] A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
    \\
    &= -i\bar{g}^2 \int_k  \frac{ 4 p^\rho k^\sigma \left( \delta_{\rho\mu}\delta_{\sigma\nu} - \delta_{\rho\sigma}\delta_{\mu\nu} + \delta_{\rho\nu}\delta_{\mu\sigma} \right) A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}
    \\
    &= -4i\bar{g}^2 \int_k  \frac{\left( p_\mu k_\nu - p_\sigma k^\sigma \delta_{\mu\nu} + p_\nu k_\mu \right) A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2}  \right] \frac{1}{q^2}.
\end{align*}
$$

Aqui $p_\mu k_\nu = p_\nu k_\mu$ quando levantarmos/abaixarmos índices, ou realizarmos os produtos internos, então já podemos substituir esses termos por $2p_\mu k_\nu$. Fazendo a distributiva com o propagador do Glúon, tem-se
$$
\begin{align*}
    &= -4i\bar{g}^2 \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[2p_\mu k_\nu - (p \cdot k) \delta_{\mu\nu} \right] \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2} \right] \frac{1}{q^2} \\
    &= -4i\bar{g}^2 \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[2\Delta_T(p \cdot k) - 4\Delta_T (p \cdot k) + 2\left(\alpha - \Delta_T\right) \frac{(p \cdot q)(k \cdot q)}{q^2} - \left(\alpha - \Delta_T\right) \frac{(p \cdot k)q^2}{q^2} \right] \frac{1}{q^2}
    \\
    &= -4i\bar{g}^2 \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left\{ -2(p \cdot k) \Delta_T +\left[ 2\frac{(p \cdot q)(k \cdot q)}{q^2} - (p \cdot k) \right] \left(\alpha - \Delta_T\right) \right\} \frac{1}{q^2},
\end{align*}
$$

sendo que segundo termo da DSE possui 3 matrizes de Dirac, então seu traço é zero. Juntando ambos os lados:
$$
\begin{equation}
    4ip^2 A(p^2) - 4ip^2 = -4i\bar{g}^2 \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left\{ -2(p \cdot k) \Delta_T +\left[ 2\frac{(p \cdot q)(k \cdot q)}{q^2} - (p \cdot k) \right] \left(\alpha - \Delta_T\right) \right\} \frac{1}{q^2}
\end{equation}
$$

e, reorganizando, ficamos com
$$
\begin{equation}
    A(p^2) = 1 - \frac{\bar{g}^2}{p^2} \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left\{ -2(p \cdot k) \Delta_T + \left[ 2\frac{(p \cdot q)(k \cdot q)}{q^2} - (p \cdot k) \right] \left(\alpha - \Delta_T\right) \right\} \frac{1}{q^2},
\end{equation}
$$

ou, ainda,
$$
\begin{equation}
    A(p^2) = 1 + \frac{\bar{g}^2}{p^2} \int_k  \frac{A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \frac{1}{q^2} \left\{\left[(p \cdot k) - 2\frac{(p \cdot q)(k \cdot q)}{q^2} \right]\alpha + \left[(p \cdot k) + 2\frac{(p \cdot q)(k \cdot q)}{q^2} \right]\Delta_T \right\}.
\end{equation}
$$

Agora, multiplicamos a DSE original pela identidade
$$
\begin{align*}
    i \mathbb{I} p\!\!\!/ A(p^2) + \mathbb{I}B(p^2) - \mathbb{I} ip\!\!\!/ + \mathbb{I}m_0 &= -\bar{g}^2 \int_k  \frac{\mathbb{I} \gamma_\mu k\!\!\!/ \gamma_\nu A(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2} \right] \frac{1}{q^2}
    \\
    &\ \ \ \ + \bar{g}^2 \int_k \frac{\mathbb{I} \gamma_\mu \gamma_\nu B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2} \right] \frac{1}{q^2}
\end{align*}
$$

e então tomamos o traço. O lado esquerdo fica
$$
    i \text{tr}[p\!\!\!/ ] A(p^2) + \text{tr}[\mathbb{I}]B(p^2) - i\text{tr}[p\!\!\!/ ] - \text{tr}[\mathbb{I}]m_0 = 4B(p^2) - 4m_0
$$

enquanto que, no lado direito, o traço do primeiro termo é zero, portanto
$$
\begin{align*}
    \bar{g}^2 \int_k \frac{\text{tr}[ \gamma_\mu \gamma_\nu ] B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} &\left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2} \right] \frac{1}{q^2} \\
    &= \bar{g}^2 \int_k \frac{4\delta_{\mu\nu} B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ \Delta_T \delta^{\mu\nu} + \left(\alpha - \Delta_T\right) \frac{q^\mu q^\nu}{q^2} \right] \frac{1}{q^2} \\
    &= 4 \bar{g}^2 \int_k \frac{B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left[ 4\Delta_T + \left(\alpha - \Delta_T\right) \right] \frac{1}{q^2} \\
    &= 4 \bar{g}^2 \int_k \frac{B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left( \alpha + 3\Delta_T \right) \frac{1}{q^2}.
\end{align*}
$$

Juntando ambos os lados:
$$
\begin{equation}
    4B(p^2) - 4m_0 = 4 \bar{g}^2 \int_k \frac{B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \left( \alpha + 3\Delta_T \right) \frac{1}{q^2}
\end{equation}
$$

e, reorganizando, obtemos
$$
\begin{equation}
    B(p^2) = m_0 + \bar{g}^2 \int_k \frac{B(k^2)}{k^2 A^2(k^2) + B^2(k^2)} \frac{1}{q^2} \left( \alpha + 3\Delta_T \right).
\end{equation}
$$
