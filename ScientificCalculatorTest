import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

class ScientificCalculatorTest {

    ScientificCalculator calculator = new ScientificCalculator();

    @Test
    void testAddition() {
        assertEquals(5.0, calculator.add(2.0, 3.0));
        assertEquals(-1.0, calculator.add(-3.0, 2.0));
    }

    @Test
    void testSubtraction() {
        assertEquals(1.0, calculator.subtract(3.0, 2.0));
        assertEquals(-5.0, calculator.subtract(-3.0, 2.0));
    }

    @Test
    void testMultiplication() {
        assertEquals(6.0, calculator.multiply(2.0, 3.0));
        assertEquals(-6.0, calculator.multiply(-2.0, 3.0));
    }

    @Test
    void testDivision() {
        assertEquals(2.0, calculator.divide(6.0, 3.0));
        assertThrows(ArithmeticException.class, () -> calculator.divide(1.0, 0.0));
    }

    @Test
    void testPower() {
        assertEquals(8.0, calculator.power(2.0, 3.0));
        assertEquals(0.25, calculator.power(2.0, -2.0));
    }

    @Test
    void testSquareRoot() {
        assertEquals(3.0, calculator.squareRoot(9.0));
        assertThrows(ArithmeticException.class, () -> calculator.squareRoot(-9.0));
    }

    @Test
    void testSine() {
        assertEquals(0.0, calculator.sine(0.0), 1e-9);
        assertEquals(1.0, calculator.sine(90.0), 1e-9);
    }

    @Test
    void testCosine() {
        assertEquals(1.0, calculator.cosine(0.0), 1e-9);
        assertEquals(0.0, calculator.cosine(90.0), 1e-9);
    }

    @Test
    void testTangent() {
        assertEquals(0.0, calculator.tangent(0.0), 1e-9);
        assertThrows(ArithmeticException.class, () -> calculator.tangent(90.0));
    }
}
