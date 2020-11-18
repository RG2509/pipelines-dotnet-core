[TestClass]
    public class FibonacciTests
    {
        [TestMethod]
        //Check the first value we calculate
        public void Fibonacci_GetNthTerm_Input2_AssertResult1()
        {
            //Arrange
            int n = 2;

            //setup
            Mock<UnitTests.IMath> mockMath = new Mock<UnitTests.IMath>();
            mockMath
                .Setup(r => r.Add(It.IsAny<int>(), It.IsAny<int>()))
                .Returns((int x, int y) => x + y);
            UnitTests.Fibonacci fibonacci = new UnitTests.Fibonacci(mockMath.Object);
            //Act
            int result = fibonacci.GetNthTerm(n);

            //Assert
            Assert.AreEqual(result, 1);
        }
}
